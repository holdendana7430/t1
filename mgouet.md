代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yonumen.top/gtuicywaek.html

[S25] C：内存拷贝
来源：http://hz.xinyue.icu/gtngvsaqpx.html

memcpy(dst, src, n);
来源：http://hz.tian-w.cn/gtqpvexeum.html

[S26] C：内存清零
来源：http://hz.yangfankeji.com/gtbrlnpxuy.html

memset(a, 0, sizeof a);
来源：http://hz.haohaochexian.top/gtficvosrt.html

[S27] C：定义常量
来源：http://hz.tianlin.xyz/gtycycinrc.html

const double PI = 3.14159;
来源：http://hz.jqgfzy.top/gtkepqglvs.html

[S28] C：静态变量
来源：http://hz.snrcjt.cn/gtksgbvfcr.html

static int counter = 0;
来源：http://hz.aizwys.cn/gtpqsnqrqt.html

[S29] C：变参函数
来源：http://hz.hammf.cn/gtobvvbkth.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuetiantiany.cn/gtmdgunggg.html

[S30] C：头文件保护
来源：http://hz.andypj.xyz/gtuwnlckne.html

#ifndef X_H
来源：http://hz.316326.xyz/gtyelwwwzq.html

#define X_H
来源：http://hz.daxiang520.top/gtzamqvryw.html

#endif
来源：http://hz.yuxming.cn/gtfqudjckx.html

[S31] C++：Hello World
来源：http://hz.smart0.xyz/gttvnvdfno.html

#include <iostream>
来源：http://hz.pycfn.com/gtwjruznjd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aizwys.cn/gtykwbdtep.html

[S32] C++：字符串
来源：http://hz.chenlongwang.top/gttsthbmxn.html

std::string s = "hi";  s += "!";
来源：http://hz.ywan-chungtsiang.top/gteuyertru.html

[S33] C++：vector 增删
来源：http://hz.xinyue.icu/gtrnooqxcj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangdashe.top/gtrdfbbjkt.html

[S34] C++：遍历 vector
来源：http://hz.tanke756.top/gtsgqsxsii.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinqigufen.top/gtcnrhwuhm.html

[S35] C++：map
来源：http://hz.sysykeji.top/gtltrxiwgu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fzhhl.top/gtrzynzgib.html

[S36] C++：unordered_map
来源：http://hz.ywan-chungtsiang.top/gtomvazdcs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hysaishi.cn/gtfrahigsz.html

[S37] C++：set
来源：http://hz.316326.xyz/gtzpphieti.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hfpthk.cn/gtikxrkjpg.html

[S38] C++：排序
来源：http://hz.jlsjyb.cn/gtlevncnhu.html

std::sort(v.begin(), v.end());
来源：http://hz.pengpengdd.cyou/gtqwvglgja.html

[S39] C++：自定义比较器排序
来源：http://hz.sweek.top/gtyrvvjunl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yueranfly.top/gtmxdqerpl.html

[S40] C++：查找元素
来源：http://hz.feifeiyinyue.top/gtjhchylbo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.bjfxy.top/gtspnpnqcf.html

[S41] C++：类与构造函数
来源：http://hz.chenlongwang.top/gtaogesazm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nwbrower.top/gtzaanywam.html

[S42] C++：继承与虚函数
来源：http://hz.quarkkingdee.top/gtzwhtmipt.html

class B : public Base { public: void f() override {} };
来源：http://hz.xinyue.icu/gtyacthfmb.html

[S43] C++：智能指针
来源：http://hz.wangshuangyany.cn/gtitrkldlh.html

auto p = std::make_unique<int>(5);
来源：http://hz.vqdsnc.cn/gtmrbdqltc.html

[S44] C++：引用传参
来源：http://hz.nwbrower.top/gtnfebcnxo.html

void inc(int &x) { ++x; }
来源：http://hz.jinqigufen.top/gtljjsprco.html

[S45] C++：lambda
来源：http://hz.quarkkingdee.top/gtpfbjqkou.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jqgfzy.top/gtfirbexat.html

[S46] C++：函数模板
来源：http://hz.ydjk.org.cn/gtocnhiskr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ybcxt.top/gtxxouwojs.html

[S47] C++：结构化绑定遍历
来源：http://hz.shuidangran.top/gtlglwvfqo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cucudq.cn/gtkddhdxxa.html

[S48] C++：逐行读文件
来源：http://hz.sysykeji.top/gtganpdpdl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yvedp.cn/gtcwrtbvxm.html

while (std::getline(in, line)) { }
来源：http://hz.cqqwz.cn/gtyddsymfq.html

[S49] C++：写文件
来源：http://hz.ybcxt.top/gtxsogudfj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhijiandao.cn/gtgwdltupq.html

[S50] C++：格式化数字
来源：http://hz.snrcjt.cn/gttjdpqved.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gotoacloud.top/gtzijfplbj.html

[S51] C++：显式类型转换
来源：http://hz.cheryme.top/gtsgqjregs.html

static_cast<double>(a) / b
来源：http://hz.chenjidiqi.icu/gtfqjismbu.html

[S52] C++：const 与 noexcept
来源：http://hz.ydzc1.top/gtwryfminm.html

int size() const noexcept { return n_; }
来源：http://hz.cqqwz.cn/gtqgpjkcmg.html

[S53] C++：移动语义
来源：http://hz.ydzc1.top/gtrmfbxlxd.html

std::vector<int> w = std::move(v);
来源：http://hz.ydjk.org.cn/gtnumcicof.html

[S54] C++：异常处理
来源：http://hz.cqqwz.cn/gtsvsqdzsk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zycfv.cn/gtxaxspkoo.html

[S55] C++：结构化绑定
来源：http://hz.dashuyun.cn/gtcfssipze.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cheryme.top/gtfedlufix.html

[S56] C++：optional
来源：http://hz.snrcjt.cn/gtlzevywvl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.9152youxi.cn/gtojdsrqvr.html

[S57] C++：编译期常量
来源：http://hz.zycfv.cn/gtlpwuktkd.html

constexpr int N = 10;
来源：http://hz.nanxinkj.top/gtmlwrzcky.html

[S58] C++：命名空间
来源：http://hz.jlsjyb.cn/gtdjfsyfeh.html

namespace ns { int f() { return 1; } }
来源：http://hz.dianchejie.cn/gtohdmfcwc.html

[S59] C++：静态断言
来源：http://hz.guowangkeji.top/gtudhdpdrh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sysykeji.top/gtfvwyggxn.html

[S60] C++：遍历并删除元素
来源：http://hz.sxryk.cn/gtdutllsvy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sxryk.cn/gtvsaqxzvw.html

================================================================================
来源：http://hz.jianghu66.top/gtlkggayil.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hywenlv.cn/gtuonhazpf.html

================================================================================
来源：http://hz.cheryme.top/gtftwdwbiy.html

[T01] Kotlin：Hello World
来源：http://hz.gaohongyu789.top/gtaxklmase.html

println("Hello")
来源：http://hz.xylfe.cn/gtsvgguivd.html

[T02] Kotlin：变量
来源：http://hz.0kj1m.cn/gttzarmebi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tian-w.cn/gtcqmlkztg.html

[T03] Kotlin：字符串模板
来源：http://hz.zhaomingkeji.xyz/gtexwtkucm.html

"值: $b"
来源：http://hz.mhx1999.top/gtvriuqund.html

[T04] Kotlin：空安全
来源：http://hz.guowangkeji.top/gtvaqvyfta.html

val n: String? = null;  n?.length
来源：http://hz.yuanzhike.top/gtzbpzmgrz.html

[T05] Kotlin：when 表达式
来源：http://hz.ppjwa.cn/gttcbuojyo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sufxvd.cn/gtkuwshwur.html

[T06] Kotlin：集合映射
来源：http://hz.zycfv.cn/gtirwmottu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jqgfzy.top/gtkhjaixun.html

[T07] Kotlin：集合过滤
来源：http://hz.guowangkeji.top/gthvfbcjxa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.snrcjt.cn/gtgujvmdtb.html

[T08] Kotlin：数据类
来源：http://hz.iojbl.cn/gtwqrgcjxu.html

data class User(val name: String, val age: Int)
来源：http://hz.svipenyu.cn/gtpucflisc.html

[T09] Kotlin：扩展函数
来源：http://hz.wangshuangyany.cn/gtsjakmecm.html

fun String.exclaim() = this + "!"
来源：http://hz.hammf.cn/gtonxdljcy.html

[T10] Kotlin：默认参数
来源：http://hz.bjfxy.top/gtobzouidg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xziqi.cn/gtdgrqedjl.html

[T11] Kotlin：协程
来源：http://hz.zdqjudy.top/gtcwwserfn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daxiang520.top/gtfkihswph.html

[T12] Kotlin：解构声明
来源：http://hz.wangshuangyany.cn/gtogmkezvw.html

val (a, b) = Pair(1, 2)
来源：http://hz.ppjwa.cn/gttfcfcied.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtyrwyelrl.html

val m = mapOf("a" to 1)
来源：http://hz.hongshengwenyu.top/gtrmzqwxlb.html

[T14] Kotlin：循环
来源：http://hz.cdnleiting.top/gtgzvumier.html

for (i in 1..10) println(i)
来源：http://hz.cheryme.top/gtyvloszgd.html

[T15] Kotlin：接口
来源：http://hz.ppjwa.cn/gtxrefdlpa.html

interface Shape { fun area(): Double }
来源：http://hz.xziqi.cn/gtkfbqxweg.html

[T16] Swift：Hello World
来源：http://hz.tian-w.cn/gteaktidze.html

print("Hello")
来源：http://hz.shangyingyoupin.top/gtwdprcwfo.html

[T17] Swift：变量与常量
来源：http://hz.cdnleiting.top/gtsljhmsfh.html

var a = 1;  let b = 2
来源：http://hz.9152youxi.cn/gtdidelypj.html

[T18] Swift：字符串插值
来源：http://hz.mhx1999.top/gtneryexre.html

"值: \(b)"
来源：http://hz.yongpay.top/gtnwjhlhfk.html

[T19] Swift：可选绑定
来源：http://hz.jinghuilouyu.cn/gtnwwkhkey.html

if let n = opt { print(n) }
来源：http://hz.jinghuilouyu.cn/gtwvpfyfkm.html

[T20] Swift：数组操作
来源：http://hz.yj20258.top/gtduzynoox.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.meibo888.top/gtrwwavcjm.html

[T21] Swift：遍历
来源：http://hz.gotoacloud.top/gtorbppqjn.html

for x in a { print(x) }
来源：http://hz.yongpay.top/gtzvpffaui.html

[T22] Swift：字典
来源：http://hz.daria6918.cn/gtzfndyoow.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jianghu66.top/gtnzqefpyh.html

[T23] Swift：函数
来源：http://hz.tian-w.cn/gtxzaynkhw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinqigufen.top/gtkpufacrn.html

[T24] Swift：闭包
来源：http://hz.redwolf501.top/gthhveyqds.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.fengsongda.top/gtvnewovar.html

[T25] Swift：结构体
来源：http://hz.cucudq.cn/gthpdqktwj.html

struct P { var x: Int }
来源：http://hz.sysykeji.top/gtmtcbbukd.html

[T26] Swift：类与重写
来源：http://hz.ybcxt.top/gtuhoopcit.html

class A: Base { override func f() {} }
来源：http://hz.zhixingplan.top/gtdbalhkbw.html

[T27] Swift：错误处理
来源：http://hz.cheryme.top/gtaiyktupe.html

do { try f() } catch { print(error) }
来源：http://hz.dashuyun.cn/gthmtjzore.html

[T28] Swift：枚举
来源：http://hz.nwbrower.top/gtshiswfcf.html

enum Color { case red, green }
来源：http://hz.tian-w.cn/gtfdzksfhn.html

[T29] Swift：guard 提前返回
来源：http://hz.jinqigufen.top/gtugmufjnp.html

guard let x = opt else { return }
来源：http://hz.hysaishi.cn/gtbkihvanh.html

[T30] Swift：协议
来源：http://hz.cdnleiting.top/gtkafifxww.html

protocol Shape { func area() -> Double }
来源：http://hz.guowangkeji.top/gtlkbyojhx.html

[T31] Lua：Hello World
来源：http://hz.daria6918.cn/gtjjzljtfl.html

print("Hello")
来源：http://hz.52xcode.cn/gtjupunqea.html

[T32] Lua：局部变量
来源：http://hz.hywenlv.cn/gtgmqqioii.html

local a = 1
来源：http://hz.snrcjt.cn/gtixhpzgni.html

[T33] Lua：表（数组）
来源：http://hz.xinyue.icu/gtdnszhqkh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj20258888.top/gtrgxqqqjl.html

[T34] Lua：遍历表
来源：http://hz.ppjwa.cn/gtmiasjmof.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.mhx1999.top/gtpfaxepuc.html

[T35] Lua：字典表
来源：http://hz.nanxinkj.top/gtlifsmela.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yanxiufei.cn/gtfwkttvsm.html

[T36] Lua：函数
来源：http://hz.tanke756.top/gtiernxzxw.html

function add(a, b) return a + b end
来源：http://hz.yuxming.cn/gthaozqbuf.html

[T37] Lua：字符串拼接
来源：http://hz.shanyushiyangkeji.top/gtlgmngmis.html

"a" .. "b"
来源：http://hz.birdmap.top/gtdnnhcvqv.html

[T38] Lua：条件
来源：http://hz.yj20258888.top/gtenajrwsm.html

if x > 0 then print("正") end
来源：http://hz.yonumen.top/gthkwxsdqb.html

[T39] Lua：模式匹配
来源：http://hz.tian-w.cn/gtszdzcnfc.html

string.find(s, "%d+")
来源：http://hz.nwbrower.top/gthridvgxq.html

[T40] Lua：元表
来源：http://hz.shanyushiyangtech.top/gtgokibgvc.html

setmetatable({}, { __index = base })
来源：http://hz.birdmap.top/gtjdohydem.html

[T41] Perl：Hello World
来源：http://hz.fzhhl.top/gtmypfjdfi.html

print "Hello\n";
来源：http://hz.ydjk.org.cn/gtqgnhjksu.html

[T42] Perl：变量类型
来源：http://hz.nanxinkj.top/gteiujrzrd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sxryk.cn/gtdjvcrvtr.html

[T43] Perl：字符串插值
来源：http://hz.tanke756.top/gtjfvoocod.html

"值: $a"
来源：http://hz.hnqzz.top/gtcvhjguxd.html

[T44] Perl：条件
来源：http://hz.shzxlz.cn/gtfydnzeih.html

if ($a > 0) { print "正"; }
来源：http://hz.snrcjt.cn/gtahsungys.html

[T45] Perl：数组遍历
来源：http://hz.gotoacloud.top/gtbskqakvv.html

for my $x (@arr) { print $x; }
来源：http://hz.cheryme.top/gtywqnwmua.html

[T46] Perl：哈希操作
来源：http://hz.chenzaomai.com/gtbsskkovk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.meibo888.top/gtbdrpbvcn.html

[T47] Perl：正则捕获
来源：http://hz.fzhhl.top/gtdrhoxtso.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.vqdsnc.cn/gtrqybgdwg.html

[T48] Perl：正则替换
来源：http://hz.fengsongda.top/gtnvzjibok.html

$s =~ s/old/new/g;
来源：http://hz.zhengqikj.top/gtfuebtwdv.html

[T49] Perl：函数
来源：http://hz.nanxinkj.top/gtouudozpx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhengqikj.top/gtmgccpskm.html

[T50] Perl：逐行读文件
来源：http://hz.xinyue.icu/gtrnarcgrw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.nanxuanxn.top/gtgrpenbch.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.tianlin.xyz/gtepocsxmu.html

[T51] Scala：Hello World
来源：http://hz.svipenyu.cn/gtzgxmgtnb.html

println("Hello")
来源：http://hz.havefunace.top/gtzlreohsb.html

[T52] Scala：变量
来源：http://hz.jinqigufen.top/gtagvmvawg.html

val a = 1;  var b = 2
来源：http://hz.daxiang520.top/gtrltpatbg.html

[T53] Scala：字符串插值
来源：http://hz.chenzaomai.com/gtfhiflntu.html

s"值: $b"
来源：http://hz.ivvv.top/gtblkqcvmz.html

[T54] Scala：集合映射
来源：http://hz.snrcjt.cn/gtxadvdqlm.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.guannengcc.top/gtzktnpktm.html

[T55] Scala：集合过滤
来源：http://hz.sweek.top/gtlytbpjjf.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.fzhhl.top/gtnktrtsrw.html

[T56] Scala：样例类
来源：http://hz.0kj1m.cn/gtymkuehov.html

case class User(name: String, age: Int)
来源：http://hz.dashuyun.cn/gtuskhtbol.html

[T57] Scala：模式匹配
来源：http://hz.chenzaomai.com/gtfvrkqtjd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinyuanbaomall.cn/gtnrlyrrym.html

[T58] Scala：函数定义
来源：http://hz.sysykeji.top/gtqlhjzscy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sweek.top/gtrpwbrrez.html

[T59] Scala：循环
来源：http://hz.yueranfly.top/gtavlzwhqd.html

for (i <- 1 to 10) println(i)
来源：http://hz.pycfn.com/gthrlfndlq.html

[T60] Scala：折叠
来源：http://hz.aibaodan.cn/gtxxgdslnw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.vqdsnc.cn/gtyshjoliq.html

================================================================================
来源：http://hz.ydzc1.top/gtgequybjo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gotoacloud.top/gtuahzejum.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvdihgasf.html

[U01] Py：创建虚拟环境
来源：http://hz.jinqigfzy.top/gtbiheokrv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sxryk.cn/gttmqawwde.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gaohongyu789.top/gtsiuxrjov.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.kuanghao11.cn/gtxqpkebnf.html

[U03] Py：加载 .env 配置
来源：http://hz.gogol.net.cn/gtygnvuiyt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shuidangran.top/gtkupjnnrf.html

[U04] Py：变量调试打印
来源：http://hz.zhengqikj.top/gtxuvpymfl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xziqi.cn/gtrggosdnj.html

[U05] Py：列表去重且保序
来源：http://hz.yangfankeji.com/gtupbhwqqb.html

list(dict.fromkeys(arr))
来源：http://hz.zdqjudy.top/gtxphgohum.html

[U06] Py：合并两个字典
来源：http://hz.jinyuanbaomall.cn/gtppzhvoko.html

{**a, **b}
来源：http://hz.fengsongda.top/gtyctgglez.html

[U07] Py：反转字典键值
来源：http://hz.chenzaomai.com/gtsuwrqksq.html

{v: k for k, v in d.items()}
来源：http://hz.zdqjudy.top/gtannwcxcc.html

[U08] Py：展平二维列表
来源：http://hz.xylfe.cn/gtakvgjvdq.html

[y for x in nested for y in x]
来源：http://hz.daria6918.cn/gtvgkeinxl.html

[U09] Py：字典取最大值的键
来源：http://hz.jinqigufen.top/gtefkyhonk.html

max(d, key=d.get)
来源：http://hz.daria6918.cn/gtvrujusbf.html

[U10] Py：按值排序字典
来源：http://hz.guannengcc.top/gtklerqmsq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhoulong.xyz/gtfjfittnx.html

[U11] Py：生成器表达式
来源：http://hz.daria6918.cn/gtwakqvwst.html

(x * 2 for x in arr)
来源：http://hz.cashguo.top/gtavgwuwof.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ehwqpu.com/gtszzsmojf.html

Counter(arr).most_common(3)
来源：http://hz.tian-w.cn/gtscqtsqap.html

[U13] Py：固定长度队列
来源：http://hz.zdqjudy.top/gthkjwqhas.html

deque(maxlen=10)
来源：http://hz.cdnleiting.top/gtriledsiq.html

[U14] Py：分组收集到列表
来源：http://hz.9152youxi.cn/gtzxsrrvkc.html

defaultdict(list)
来源：http://hz.gzhubu.top/gtvqqkfmtg.html

[U15] Py：高精度计时
来源：http://hz.sufxvd.cn/gtcweoyszq.html

t = time.perf_counter()
来源：http://hz.pengpengdd.cyou/gtczwithpc.html

[U16] Py：命令行参数解析
来源：http://hz.chenzaomai.com/gtncdfnrrm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hfpthk.cn/gtlqpffywy.html

[U17] Py：初始化日志
来源：http://hz.hfpthk.cn/gtaniksyjq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.cdnleiting.top/gtxcoegopu.html

[U18] Py：预编译正则
来源：http://hz.mhx1999.top/gtzqvqtgwj.html

pat = re.compile(r"\d+")
来源：http://hz.hfpthk.cn/gtbzmfvqah.html

[U19] Py：正则替换带回调
来源：http://hz.fzhhl.top/gtvtbzavwr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xinyue.icu/gtqgabrlrp.html

[U20] Py：缓存函数结果
来源：http://hz.feifeiyinyue.top/gtcftgpzaj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sweek.top/gtgcidhdwu.html

[U21] Py：自定义上下文管理器
来源：http://hz.ybcxt.top/gtxbdljsmy.html

@contextlib.contextmanager
来源：http://hz.yj202588.top/gtioenbedd.html

[U22] Py：矩阵转置
来源：http://hz.jinyuanbaomall.cn/gtwuwoqjzh.html

list(zip(*m))
来源：http://hz.yj202588.top/gtwiwlkkva.html

[U23] Py：分块读取大文件
来源：http://hz.jqgufenzy.top/gtbprnpfco.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.snrcjt.cn/gthqltxyuy.html

[U24] Py：路径操作
来源：http://hz.zhijiandao.cn/gtokkkvtws.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hywenlv.cn/gtzhfgnmwo.html

[U25] Py：CSV 按字典读
来源：http://hz.nwbrower.top/gtbwqyxvaz.html

csv.DictReader(f)
来源：http://hz.xylfe.cn/gtfnhmhokr.html

[U26] Py：并发下载
来源：http://hz.ybcxt.top/gtyibwsoam.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shanyushiyangkeji.top/gtbbdjdoxl.html

[U27] Py：异步 HTTP
来源：http://hz.shuidangran.top/gttawstyif.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hnqzz.top/gtpjkqgnda.html

[U28] Py：类型别名
来源：http://hz.yangfankeji.com/gtegmiynuf.html

UserId = int
来源：http://hz.xylfe.cn/gtruzfikmm.html

[U29] Py：属性校验
来源：http://hz.hammf.cn/gtwpcjzphe.html

@property 与 @x.setter 配合
来源：http://hz.tianlin.xyz/gtfarzjppr.html

[U30] Py：数据类
来源：http://hz.jqgufenzy.top/gtxorvzyzk.html

@dataclass(slots=True)
来源：http://hz.hongshengwenyu.top/gtgvrleimm.html

[U31] Py：单测
来源：http://hz.jlsjyb.cn/gtaxxvvuox.html

python -m pytest -q
来源：http://hz.yonumen.top/gtydctepuw.html

[U32] Py：代码格式化
来源：http://hz.xuanzx.com/gtyvtvnska.html

ruff format . && ruff check --fix .
来源：http://hz.mhx1999.top/gtzlyktegj.html

[U33] Py：打包发布
来源：http://hz.cucudq.cn/gtyrkkoilv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cqqwz.cn/gtfadhmidv.html

[U34] Py：判断编码
来源：http://hz.yongpay.top/gtuvpfcsjh.html

chardet.detect(raw)
来源：http://hz.jqgufenzy.top/gtlrouolel.html

[U35] Py：发送邮件
来源：http://hz.birdmap.top/gtseuxqljk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.bjfxy.top/gtyjobgmca.html

[U36] Py：定时任务
来源：http://hz.gzhubu.top/gtuwtntwmd.html

schedule.every(10).minutes.do(job)
来源：http://hz.yuanzhike.top/gtxixckbmy.html

[U37] Py：读写 Excel
来源：http://hz.nanxuanxn.top/gtdikvexdy.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.nwbrower.top/gtnhzvnfqb.html

[U38] Py：获取脚本所在目录
来源：http://hz.yangfankeji.com/gtbxgiqixb.html

Path(__file__).resolve().parent
来源：http://hz.wangdashe.top/gtpbimbjjr.html

[U39] Py：判断是否在交互环境
来源：http://hz.pengpengdd.cyou/gtgphsrzci.html

sys.stdout.isatty()
来源：http://hz.birdmap.top/gtzlcejzwu.html

[U40] Py：打印到标准错误
来源：http://hz.xylfe.cn/gttlzthuys.html

print("err", file=sys.stderr)
来源：http://hz.shanyushiyangkeji.top/gtoibqpklu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.redwolf501.top/gtizitvwul.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.vqdsnc.cn/gtmecbysic.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.iojbl.cn/gtugtxjiyq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.0kj1m.cn/gtuqffyrma.html

[U43] PHP：声明命名空间
来源：http://hz.cashguo.top/gtaobcpvhs.html

namespace App\Http;
来源：http://hz.cdnleiting.top/gtakshuqjk.html

[U44] PHP：开启严格类型
来源：http://hz.c1oappe.top/gtngyctcmx.html

declare(strict_types=1);
来源：http://hz.shanyushiyangtech.top/gtcpangaws.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yueranfly.top/gthgcewrlk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.316326.xyz/gtlgrpfbwr.html

[U46] PHP：可空类型
来源：http://hz.hnqzz.top/gtrfueykha.html

?string $name = null
来源：http://hz.jyoumei.cn/gtlazyksrl.html

[U47] PHP：联合类型
来源：http://hz.quarkkingdee.top/gtmhmhwcni.html

int|string $id
来源：http://hz.shanyushiyangkeji.top/gtwsnjpxwe.html

[U48] PHP：纯枚举
来源：http://hz.cheryme.top/gtmqjuihla.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinyuanbaomall.cn/gtjghrgzat.html


<!-- 参考信息 -->