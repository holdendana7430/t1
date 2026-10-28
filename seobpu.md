代发 wailian999

memset(a, 0, sizeof a);
来源：http://hz.sweek.top/gtbvsfjjdu.html

[S27] C：定义常量
来源：http://hz.chenlongwang.top/gtwugxwgqh.html

const double PI = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtgifmqrnh.html

[S28] C：静态变量
来源：http://hz.daria6918.cn/gtkxbndrkz.html

static int counter = 0;
来源：http://hz.jlsjyb.cn/gtvbuxlvxd.html

[S29] C：变参函数
来源：http://hz.xylfe.cn/gtiukiamqx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.0kj1m.cn/gtvsbudzps.html

[S30] C：头文件保护
来源：http://hz.andypj.xyz/gttyregeee.html

#ifndef X_H
来源：http://hz.pengpengdd.cyou/gtazpabiwq.html

#define X_H
来源：http://hz.xingfuxueyuan.xyz/gtixktinje.html

#endif
来源：http://hz.jinqigufen.top/gtrzjitetg.html

[S31] C++：Hello World
来源：http://hz.nanxinkj.top/gtduuridlt.html

#include <iostream>
来源：http://hz.redwolf501.top/gtzzrktgxi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cqqwz.cn/gtheuerwkc.html

[S32] C++：字符串
来源：http://hz.jinqigfzy.top/gtckdrtuyg.html

std::string s = "hi";  s += "!";
来源：http://hz.ivvv.top/gtmjkgkwwu.html

[S33] C++：vector 增删
来源：http://hz.yuxming.cn/gtgkvieckc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.52xcode.cn/gtxcaczgmh.html

[S34] C++：遍历 vector
来源：http://hz.havefunace.top/gtlrjreuyh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jiagoushi.top/gtugyyoktm.html

[S35] C++：map
来源：http://hz.hnxiangtu.top/gtiksfyrhv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.smart0.xyz/gtikufepyf.html

[S36] C++：unordered_map
来源：http://hz.snrcjt.cn/gttoqdbelq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtffyrjcsb.html

[S37] C++：set
来源：http://hz.tanke756.top/gtvwbfgkxi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.wangshuangyany.cn/gtxqriizuf.html

[S38] C++：排序
来源：http://hz.xuetiantiany.cn/gtjbhfdczn.html

std::sort(v.begin(), v.end());
来源：http://hz.xinyue.icu/gtomtmuhav.html

[S39] C++：自定义比较器排序
来源：http://hz.xylfe.cn/gtfsaixolp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhiwuduotai.top/gtylkiqzwy.html

[S40] C++：查找元素
来源：http://hz.tianlin.xyz/gtfihqqtbs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.pycfn.com/gtcxzlhgsq.html

[S41] C++：类与构造函数
来源：http://hz.jinyuanbaomall.cn/gteberyzef.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.316326.xyz/gtjsnuzhvb.html

[S42] C++：继承与虚函数
来源：http://hz.vqdsnc.cn/gtimkwxxhs.html

class B : public Base { public: void f() override {} };
来源：http://hz.fengsongda.top/gtbrhyawve.html

[S43] C++：智能指针
来源：http://hz.shuidangran.top/gtnzpovetm.html

auto p = std::make_unique<int>(5);
来源：http://hz.cheryme.top/gtkggxovhr.html

[S44] C++：引用传参
来源：http://hz.52xcode.cn/gtbiiofrds.html

void inc(int &x) { ++x; }
来源：http://hz.9152youxi.cn/gtmaxwidqv.html

[S45] C++：lambda
来源：http://hz.sxryk.cn/gtegcaojrm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tanke756.top/gtzwbhopuk.html

[S46] C++：函数模板
来源：http://hz.hywenlv.cn/gtvmpescwc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.redwolf501.top/gtoqetcmrn.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenjidiqi.icu/gtlaifppfy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.c1oappe.top/gtchikiuzr.html

[S48] C++：逐行读文件
来源：http://hz.xinyue.icu/gtavixqvff.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.fzhhl.top/gthcmstbnr.html

while (std::getline(in, line)) { }
来源：http://hz.jinqigfzy.top/gtsmvlnlfi.html

[S49] C++：写文件
来源：http://hz.pycfn.com/gtqcvwdjyc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zdqjudy.top/gtlbzsvpco.html

[S50] C++：格式化数字
来源：http://hz.sweek.top/gttnxurdvy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.havefunace.top/gtvlcnnwsd.html

[S51] C++：显式类型转换
来源：http://hz.zhongyouzk.top/gtfohybmsk.html

static_cast<double>(a) / b
来源：http://hz.xylfe.cn/gtjlsivuea.html

[S52] C++：const 与 noexcept
来源：http://hz.havefunace.top/gtxvkrlgnz.html

int size() const noexcept { return n_; }
来源：http://hz.sxryk.cn/gtckktwuod.html

[S53] C++：移动语义
来源：http://hz.feifeiyinyue.top/gtyqrgsxhn.html

std::vector<int> w = std::move(v);
来源：http://hz.hongshengwenyu.top/gtthunqngn.html

[S54] C++：异常处理
来源：http://hz.ydjk.org.cn/gteasooysm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yonumen.top/gtvzkojleh.html

[S55] C++：结构化绑定
来源：http://hz.c1oappe.top/gtipxzyiqf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shanyushiyangkeji.top/gtvfvxlqyk.html

[S56] C++：optional
来源：http://hz.andypj.xyz/gtbtoxsxnp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhijiandao.cn/gtcqkadtic.html

[S57] C++：编译期常量
来源：http://hz.chenlongwang.top/gtucxelago.html

constexpr int N = 10;
来源：http://hz.yueranfly.top/gtwujwqsue.html

[S58] C++：命名空间
来源：http://hz.hnxiangtu.top/gtjggzfbht.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinqigfzy.top/gthwqhkorz.html

[S59] C++：静态断言
来源：http://hz.hysaishi.cn/gtgfqexqrw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxuanxn.top/gtxpcuorbv.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangkeji.top/gtutaodhti.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xinyue.icu/gtexgtrdnp.html

================================================================================
来源：http://hz.316326.xyz/gtodtjaycl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sufxvd.cn/gtinyajigf.html

================================================================================
来源：http://hz.yvedp.cn/gtpmsdcxoo.html

[T01] Kotlin：Hello World
来源：http://hz.hywenlv.cn/gtiofvwzft.html

println("Hello")
来源：http://hz.shanyushiyangtech.top/gtojxhuvvv.html

[T02] Kotlin：变量
来源：http://hz.nwbrower.top/gtggsuhkpu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.iojbl.cn/gtvgmeedjv.html

[T03] Kotlin：字符串模板
来源：http://hz.hnqzz.top/gtnnwdptrv.html

"值: $b"
来源：http://hz.svipenyu.cn/gtoygtnlzm.html

[T04] Kotlin：空安全
来源：http://hz.smart0.xyz/gtmehawmes.html

val n: String? = null;  n?.length
来源：http://hz.birdmap.top/gtcxkeowhl.html

[T05] Kotlin：when 表达式
来源：http://hz.quarkkingdee.top/gtepnwhujr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhijiandao.cn/gtdcyfkcgt.html

[T06] Kotlin：集合映射
来源：http://hz.cheryme.top/gtyzmdnkrq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.pengpengdd.cyou/gtutzyflor.html

[T07] Kotlin：集合过滤
来源：http://hz.jinghuilouyu.cn/gtnlkponla.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cashguo.top/gtljodhcvb.html

[T08] Kotlin：数据类
来源：http://hz.xziqi.cn/gtxnfqspfb.html

data class User(val name: String, val age: Int)
来源：http://hz.yuanzhike.top/gtrfvwmsbb.html

[T09] Kotlin：扩展函数
来源：http://hz.cheryme.top/gtgnzjmgmj.html

fun String.exclaim() = this + "!"
来源：http://hz.hongshengwenyu.top/gtrynlzdma.html

[T10] Kotlin：默认参数
来源：http://hz.hammf.cn/gtwtggsbhd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xziqi.cn/gtbfefhxal.html

[T11] Kotlin：协程
来源：http://hz.yj20258888.top/gtdsqyumjk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.fengsongda.top/gthfidcdsm.html

[T12] Kotlin：解构声明
来源：http://hz.xziqi.cn/gtdonvrnqx.html

val (a, b) = Pair(1, 2)
来源：http://hz.birdmap.top/gtyqeobpdv.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258.top/gtokoucoqj.html

val m = mapOf("a" to 1)
来源：http://hz.redwolf501.top/gtolfojhgd.html

[T14] Kotlin：循环
来源：http://hz.xuanzx.com/gtzttusfha.html

for (i in 1..10) println(i)
来源：http://hz.zhoulong.xyz/gtmpfxjjmk.html

[T15] Kotlin：接口
来源：http://hz.zhijiandao.cn/gtrtznugji.html

interface Shape { fun area(): Double }
来源：http://hz.quarkkingdee.top/gthonuhowg.html

[T16] Swift：Hello World
来源：http://hz.kuanghao11.cn/gtmlynvubz.html

print("Hello")
来源：http://hz.tanke756.top/gtkqglwtvm.html

[T17] Swift：变量与常量
来源：http://hz.cdnleiting.top/gtmgriosmr.html

var a = 1;  let b = 2
来源：http://hz.haohaochexian.top/gtjiuwavaq.html

[T18] Swift：字符串插值
来源：http://hz.dianchejie.cn/gtrxunuxgq.html

"值: \(b)"
来源：http://hz.hongshengwenyu.top/gtoepmjmwp.html

[T19] Swift：可选绑定
来源：http://hz.0kj1m.cn/gtvruzuoaf.html

if let n = opt { print(n) }
来源：http://hz.smart0.xyz/gtohnkgplm.html

[T20] Swift：数组操作
来源：http://hz.wangshuangyany.cn/gtxsmmrbvj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jqgufenzy.top/gtjflpfudf.html

[T21] Swift：遍历
来源：http://hz.zhixingplan.top/gtzaubcqlj.html

for x in a { print(x) }
来源：http://hz.guannengcc.top/gtsepjrhat.html

[T22] Swift：字典
来源：http://hz.yangfankeji.com/gtcchmrsgr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sxryk.cn/gtogyyhczk.html

[T23] Swift：函数
来源：http://hz.shangyingyoupin.top/gtwyjmrlte.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinqigfzy.top/gthzzdutbg.html

[T24] Swift：闭包
来源：http://hz.hnxiangtu.top/gtzcewvxnp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jqgfzy.top/gtknigmycm.html

[T25] Swift：结构体
来源：http://hz.kuanghao11.cn/gthszuvude.html

struct P { var x: Int }
来源：http://hz.pengpengdd.cyou/gtfsmhhzsg.html

[T26] Swift：类与重写
来源：http://hz.tanke756.top/gtovohaoab.html

class A: Base { override func f() {} }
来源：http://hz.zhijiandao.cn/gtgtilhsrm.html

[T27] Swift：错误处理
来源：http://hz.havefunace.top/gtxcgfxofg.html

do { try f() } catch { print(error) }
来源：http://hz.zhixingplan.top/gtbbgktuns.html

[T28] Swift：枚举
来源：http://hz.yvedp.cn/gtecycctcb.html

enum Color { case red, green }
来源：http://hz.cucudq.cn/gtgodmmejv.html

[T29] Swift：guard 提前返回
来源：http://hz.xingfuxueyuan.xyz/gtdmhbebzc.html

guard let x = opt else { return }
来源：http://hz.zhongyouzk.top/gtanchurrm.html

[T30] Swift：协议
来源：http://hz.sweek.top/gtpxxnaxso.html

protocol Shape { func area() -> Double }
来源：http://hz.yuanzhike.top/gtpexpauuy.html

[T31] Lua：Hello World
来源：http://hz.52xcode.cn/gthlrzdxwm.html

print("Hello")
来源：http://hz.nwbrower.top/gtetptntef.html

[T32] Lua：局部变量
来源：http://hz.shanyushiyangkeji.top/gtyckozrci.html

local a = 1
来源：http://hz.aibaodan.cn/gthadmvkik.html

[T33] Lua：表（数组）
来源：http://hz.52xcode.cn/gtvqrxguyg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.fengsongda.top/gtokhezebx.html

[T34] Lua：遍历表
来源：http://hz.daxiang520.top/gtcgewiqqu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.haohaochexian.top/gtmgpirfgq.html

[T35] Lua：字典表
来源：http://hz.sysykeji.top/gtpxcavlmw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.chenzaomai.com/gtrvpvhaea.html

[T36] Lua：函数
来源：http://hz.jinqigufen.top/gtptgvuxvn.html

function add(a, b) return a + b end
来源：http://hz.sysykeji.top/gtqwavilzo.html

[T37] Lua：字符串拼接
来源：http://hz.xylfe.cn/gtmqadozei.html

"a" .. "b"
来源：http://hz.jiagoushi.top/gtiknuhspn.html

[T38] Lua：条件
来源：http://hz.nanxuanxn.top/gtulhxmmpj.html

if x > 0 then print("正") end
来源：http://hz.cqqwz.cn/gtidlqixwt.html

[T39] Lua：模式匹配
来源：http://hz.xingfuxueyuan.xyz/gtdffvptbw.html

string.find(s, "%d+")
来源：http://hz.316326.xyz/gtklwdkrpa.html

[T40] Lua：元表
来源：http://hz.svipenyu.cn/gtwxkukdex.html

setmetatable({}, { __index = base })
来源：http://hz.tianlin.xyz/gtptbjsprm.html

[T41] Perl：Hello World
来源：http://hz.wangdashe.top/gtstotsoya.html

print "Hello\n";
来源：http://hz.yueranfly.top/gtdyxfpjtz.html

[T42] Perl：变量类型
来源：http://hz.smart0.xyz/gtwdayviqk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhaomingkeji.xyz/gtabectjqb.html

[T43] Perl：字符串插值
来源：http://hz.shuidangran.top/gtfifxkbjt.html

"值: $a"
来源：http://hz.fengsongda.top/gterxfoopt.html

[T44] Perl：条件
来源：http://hz.haohaochexian.top/gtkqdsnfjc.html

if ($a > 0) { print "正"; }
来源：http://hz.nwbrower.top/gtieybknbt.html

[T45] Perl：数组遍历
来源：http://hz.wangshuangyany.cn/gtrypyohsi.html

for my $x (@arr) { print $x; }
来源：http://hz.hnxiangtu.top/gtyyvmhjcq.html

[T46] Perl：哈希操作
来源：http://hz.tanke756.top/gtjtryqbzx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.wangdashe.top/gtuxmnmutr.html

[T47] Perl：正则捕获
来源：http://hz.yonumen.top/gtfnltcayu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.chenzaomai.com/gtxlabmcjl.html

[T48] Perl：正则替换
来源：http://hz.gaohongyu789.top/gtqmgeojhr.html

$s =~ s/old/new/g;
来源：http://hz.yanxiufei.cn/gteizclwqd.html

[T49] Perl：函数
来源：http://hz.yangfankeji.com/gtsyylowob.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sysykeji.top/gtzzreumfb.html

[T50] Perl：逐行读文件
来源：http://hz.ppjwa.cn/gtusiyqjzi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yueranfly.top/gtrqahrtir.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.daxiang520.top/gtvmvbmiot.html

[T51] Scala：Hello World
来源：http://hz.jinqigufen.top/gtgmfmnyqf.html

println("Hello")
来源：http://hz.yj202588.top/gtvkoutrdm.html

[T52] Scala：变量
来源：http://hz.jqgufenzy.top/gtvapllvyl.html

val a = 1;  var b = 2
来源：http://hz.hnqzz.top/gtcsqbcnqo.html

[T53] Scala：字符串插值
来源：http://hz.meibo888.top/gtzxuxnzoi.html

s"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gtpqjldgod.html

[T54] Scala：集合映射
来源：http://hz.yj202588.top/gthcnmqfzn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shanyushiyangkeji.top/gtueelaflv.html

[T55] Scala：集合过滤
来源：http://hz.quarkkingdee.top/gtoalhytwr.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dashuyun.cn/gtgdgdycdz.html

[T56] Scala：样例类
来源：http://hz.chenlongwang.top/gtvqbgesza.html

case class User(name: String, age: Int)
来源：http://hz.smart0.xyz/gtiyzlafiv.html

[T57] Scala：模式匹配
来源：http://hz.feifeiyinyue.top/gtlefuavdy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hongshengwenyu.top/gtyixdxbjv.html

[T58] Scala：函数定义
来源：http://hz.jyoumei.cn/gtmygzneqk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yangfankeji.com/gtoufolwsv.html

[T59] Scala：循环
来源：http://hz.dianchejie.cn/gtucpmgosc.html

for (i <- 1 to 10) println(i)
来源：http://hz.gzhubu.top/gtxihfjttc.html

[T60] Scala：折叠
来源：http://hz.sweek.top/gtgbspgakd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.dashuyun.cn/gttojayvsd.html

================================================================================
来源：http://hz.ppjwa.cn/gtymptujof.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yanxiufei.cn/gtwxntaetc.html

================================================================================
来源：http://hz.zhongyouzk.top/gtesdalyvv.html

[U01] Py：创建虚拟环境
来源：http://hz.ywan-chungtsiang.top/gtapsstqjs.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.nanxinkj.top/gtngfhnwwv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.haohaochexian.top/gtxhieycjs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jyoumei.cn/gtbkoyopev.html

[U03] Py：加载 .env 配置
来源：http://hz.mhx1999.top/gthoujtqfm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shzxlz.cn/gtaagqvkmu.html

[U04] Py：变量调试打印
来源：http://hz.c1oappe.top/gtjccmkfyq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhijiandao.cn/gtftunnywx.html

[U05] Py：列表去重且保序
来源：http://hz.aibaodan.cn/gtxflbnanq.html

list(dict.fromkeys(arr))
来源：http://hz.zhoulong.xyz/gtrrsstvev.html

[U06] Py：合并两个字典
来源：http://hz.nanxuanxn.top/gthnnskijc.html

{**a, **b}
来源：http://hz.xylfe.cn/gtkqrwruog.html

[U07] Py：反转字典键值
来源：http://hz.sysykeji.top/gtwfwwyale.html

{v: k for k, v in d.items()}
来源：http://hz.guannengcc.top/gtkmteaown.html

[U08] Py：展平二维列表
来源：http://hz.aizwys.cn/gtnbyiotik.html

[y for x in nested for y in x]
来源：http://hz.quarkkingdee.top/gtwnqvwbhr.html

[U09] Py：字典取最大值的键
来源：http://hz.haohaochexian.top/gtqmypskpl.html

max(d, key=d.get)
来源：http://hz.guannengcc.top/gtbwapkbsm.html

[U10] Py：按值排序字典
来源：http://hz.sysykeji.top/gtzoapmosz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.snrcjt.cn/gtesgrikdo.html

[U11] Py：生成器表达式
来源：http://hz.yj20258888.top/gtfwwluqzl.html

(x * 2 for x in arr)
来源：http://hz.sweek.top/gthjglgler.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yangfankeji.com/gtaidbsipb.html

Counter(arr).most_common(3)
来源：http://hz.dianchejie.cn/gtadammirh.html

[U13] Py：固定长度队列
来源：http://hz.ydjk.org.cn/gtcdtkhjjh.html

deque(maxlen=10)
来源：http://hz.jinghuilouyu.cn/gtbmpqvkhf.html

[U14] Py：分组收集到列表
来源：http://hz.zhaomingkeji.xyz/gtffzcaras.html

defaultdict(list)
来源：http://hz.cheryme.top/gtekculcfm.html

[U15] Py：高精度计时
来源：http://hz.cdnleiting.top/gtuajojtbc.html

t = time.perf_counter()
来源：http://hz.ydjk.org.cn/gtrjxcahyz.html

[U16] Py：命令行参数解析
来源：http://hz.zhaomingkeji.xyz/gturkgwsrn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.haohaochexian.top/gtedsnwsjz.html

[U17] Py：初始化日志
来源：http://hz.fengsongda.top/gtflnkwigi.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yangfankeji.com/gtflpomouj.html

[U18] Py：预编译正则
来源：http://hz.kuanghao11.cn/gtsvliisip.html

pat = re.compile(r"\d+")
来源：http://hz.52xcode.cn/gtugvcrydb.html

[U19] Py：正则替换带回调
来源：http://hz.dianchejie.cn/gtcwvnayun.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.guowangkeji.top/gtpssuptze.html

[U20] Py：缓存函数结果
来源：http://hz.chenlongwang.top/gtymzwgixp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hysaishi.cn/gtltvyngci.html

[U21] Py：自定义上下文管理器
来源：http://hz.fengsongda.top/gtdhjvasxy.html

@contextlib.contextmanager
来源：http://hz.xinyue.icu/gtkktytzrs.html

[U22] Py：矩阵转置
来源：http://hz.yanxiufei.cn/gtfeiuctdn.html

list(zip(*m))
来源：http://hz.dashuyun.cn/gtvkplayyp.html

[U23] Py：分块读取大文件
来源：http://hz.jlsjyb.cn/gtpgpaconc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.0kj1m.cn/gtoacyiueu.html

[U24] Py：路径操作
来源：http://hz.hysaishi.cn/gteybqodbs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hysaishi.cn/gtipvkdpgz.html

[U25] Py：CSV 按字典读
来源：http://hz.chenjidiqi.icu/gtdosfzhrv.html

csv.DictReader(f)
来源：http://hz.feifeiyinyue.top/gtryuugnvj.html

[U26] Py：并发下载
来源：http://hz.hnxiangtu.top/gtfvcufclu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cucudq.cn/gttsrohzlb.html

[U27] Py：异步 HTTP
来源：http://hz.daria6918.cn/gtcqtalabx.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xuanzx.com/gtkamwqypy.html

[U28] Py：类型别名
来源：http://hz.xziqi.cn/gtsumlunae.html

UserId = int
来源：http://hz.xziqi.cn/gtiqtnnhjq.html

[U29] Py：属性校验
来源：http://hz.svipenyu.cn/gtapdbrzhb.html

@property 与 @x.setter 配合
来源：http://hz.zhongyouzk.top/gtczkaxxvd.html

[U30] Py：数据类
来源：http://hz.pycfn.com/gtzmyfsczu.html

@dataclass(slots=True)
来源：http://hz.cqqwz.cn/gtalrmbfdn.html

[U31] Py：单测
来源：http://hz.mhx1999.top/gtyghoqkfy.html

python -m pytest -q
来源：http://hz.yj20258888.top/gtwufbiczd.html

[U32] Py：代码格式化
来源：http://hz.gogol.net.cn/gtokiwbbhp.html

ruff format . && ruff check --fix .
来源：http://hz.jyoumei.cn/gtqltluyaz.html

[U33] Py：打包发布
来源：http://hz.cqqwz.cn/gtirlafopi.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.daria6918.cn/gtydifejra.html

[U34] Py：判断编码
来源：http://hz.zhixingplan.top/gtoqglcnop.html

chardet.detect(raw)
来源：http://hz.zhixingplan.top/gtfhhaomgt.html

[U35] Py：发送邮件
来源：http://hz.feifeiyinyue.top/gtbukzrmwg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.fengsongda.top/gtohrpwoum.html

[U36] Py：定时任务
来源：http://hz.xuanzx.com/gtyjqvcuwe.html

schedule.every(10).minutes.do(job)
来源：http://hz.cqqwz.cn/gtczhfbtgq.html

[U37] Py：读写 Excel
来源：http://hz.hysaishi.cn/gthodqumkb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xuanzx.com/gtdkkqcovs.html

[U38] Py：获取脚本所在目录
来源：http://hz.bjfxy.top/gtrcxhjavn.html

Path(__file__).resolve().parent
来源：http://hz.yongpay.top/gtpujjuixs.html

[U39] Py：判断是否在交互环境
来源：http://hz.wangdashe.top/gtxvdflcna.html

sys.stdout.isatty()
来源：http://hz.shuidangran.top/gtvgtslgig.html

[U40] Py：打印到标准错误
来源：http://hz.pengpengdd.cyou/gtiowkpkez.html

print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtldzrfceu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhengqikj.top/gtoiuofuqm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ywan-chungtsiang.top/gtfmeqqizx.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.cashguo.top/gtcijocsix.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.daxiang520.top/gtptusjkkt.html

[U43] PHP：声明命名空间
来源：http://hz.meibo888.top/gtbwmffecn.html

namespace App\Http;
来源：http://hz.hfpthk.cn/gtmevpblxm.html

[U44] PHP：开启严格类型
来源：http://hz.yueranfly.top/gtesovnpyd.html

declare(strict_types=1);
来源：http://hz.c1oappe.top/gtksqqhagz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.nanxinkj.top/gtulqxebje.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgfzy.top/gtsmnskyuq.html

[U46] PHP：可空类型
来源：http://hz.xylfe.cn/gtlxirzpeb.html

?string $name = null
来源：http://hz.aibaodan.cn/gtrdjafjiq.html

[U47] PHP：联合类型
来源：http://hz.jinqigufen.top/gthctrwgwx.html

int|string $id
来源：http://hz.xylfe.cn/gttmwrxtih.html

[U48] PHP：纯枚举
来源：http://hz.yongpay.top/gteqfiggyi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cashguo.top/gtxkchuhzw.html

[U49] PHP：只读属性
来源：http://hz.dianchejie.cn/gttljsruyz.html

public readonly string $name
来源：http://hz.zhiwuduotai.top/gtvzdbmsij.html

[U50] PHP：构造器属性提升
来源：http://hz.sysykeji.top/gtyzuholjj.html

public function __construct(private int $id) {}
来源：http://hz.zhaomingkeji.xyz/gtgaggausn.html


<!-- 参考信息 -->