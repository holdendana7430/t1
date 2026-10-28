代发 wailian999

memset(a, 0, sizeof a);
来源：http://hz.yuanzhike.top/gtptwrkbhj.html

[S27] C：定义常量
来源：http://hz.chenlongwang.top/gtywkfumzp.html

const double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtypxmqcpv.html

[S28] C：静态变量
来源：http://hz.xuanzx.com/gtlgvfyrdt.html

static int counter = 0;
来源：http://hz.shanyushiyangtech.top/gtaetozsxq.html

[S29] C：变参函数
来源：http://hz.jinyuanbaomall.cn/gttmohwhev.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangtech.top/gtegcgbodz.html

[S30] C：头文件保护
来源：http://hz.cucudq.cn/gtgfkfkudf.html

#ifndef X_H
来源：http://hz.cqqwz.cn/gtkylysiis.html

#define X_H
来源：http://hz.zycfv.cn/gtzeckduwu.html

#endif
来源：http://hz.pycfn.com/gtkkffjqez.html

[S31] C++：Hello World
来源：http://hz.yj20258888.top/gtnhyxcyda.html

#include <iostream>
来源：http://hz.chenjidiqi.icu/gtytotljao.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yongpay.top/gtosvpyfms.html

[S32] C++：字符串
来源：http://hz.yj20258.top/gtzehmmnty.html

std::string s = "hi";  s += "!";
来源：http://hz.aizwys.cn/gtfkqmeqen.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtzfpjdpxq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hammf.cn/gtyuduljea.html

[S34] C++：遍历 vector
来源：http://hz.gaohongyu789.top/gtlekhntmn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shangyingyoupin.top/gtkcfxmuax.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtaidpnmzl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhongyouzk.top/gtqobppwhy.html

[S36] C++：unordered_map
来源：http://hz.pengpengdd.cyou/gtpfflchxb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yangfankeji.com/gtiyydckls.html

[S37] C++：set
来源：http://hz.xingfuxueyuan.xyz/gtpudhlatn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xingfuxueyuan.xyz/gtuohzahzw.html

[S38] C++：排序
来源：http://hz.cqqwz.cn/gtjpywqsmp.html

std::sort(v.begin(), v.end());
来源：http://hz.shanyushiyangkeji.top/gtsrzlpwrm.html

[S39] C++：自定义比较器排序
来源：http://hz.chenzaomai.com/gtrkblploy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tanke756.top/gtazynveoc.html

[S40] C++：查找元素
来源：http://hz.fengsongda.top/gttcetqzri.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.smart0.xyz/gtkrjdiczi.html

[S41] C++：类与构造函数
来源：http://hz.jinqigfzy.top/gtgofpmuze.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenjidiqi.icu/gtrpoohjyu.html

[S42] C++：继承与虚函数
来源：http://hz.nanxinkj.top/gtnivsmqqs.html

class B : public Base { public: void f() override {} };
来源：http://hz.feifeiyinyue.top/gtdkdvkrka.html

[S43] C++：智能指针
来源：http://hz.jyoumei.cn/gtxsixubef.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhaomingkeji.xyz/gtqewlucdy.html

[S44] C++：引用传参
来源：http://hz.nanxuanxn.top/gttjryfkwt.html

void inc(int &x) { ++x; }
来源：http://hz.pengpengdd.cyou/gtywflhpjy.html

[S45] C++：lambda
来源：http://hz.xingfuxueyuan.xyz/gtomyxjsnm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hfpthk.cn/gtiuaimvpd.html

[S46] C++：函数模板
来源：http://hz.yongpay.top/gttrjlgugm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sufxvd.cn/gtiypkuboy.html

[S47] C++：结构化绑定遍历
来源：http://hz.kuanghao11.cn/gtekchzwld.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hywenlv.cn/gtbwnjrojh.html

[S48] C++：逐行读文件
来源：http://hz.ivvv.top/gtxlnvbfei.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tian-w.cn/gttxlyhlnd.html

while (std::getline(in, line)) { }
来源：http://hz.hammf.cn/gtaugscthr.html

[S49] C++：写文件
来源：http://hz.pycfn.com/gthbdmslct.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.0kj1m.cn/gtajfyqlub.html

[S50] C++：格式化数字
来源：http://hz.zhoulong.xyz/gtpovbvzay.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xinyue.icu/gtgowpecfg.html

[S51] C++：显式类型转换
来源：http://hz.c1oappe.top/gteatoqyco.html

static_cast<double>(a) / b
来源：http://hz.havefunace.top/gturxufrrl.html

[S52] C++：const 与 noexcept
来源：http://hz.aizwys.cn/gtnyhvdxwa.html

int size() const noexcept { return n_; }
来源：http://hz.yuxming.cn/gttlygfmqm.html

[S53] C++：移动语义
来源：http://hz.snrcjt.cn/gtyjqggbmj.html

std::vector<int> w = std::move(v);
来源：http://hz.zhiwuduotai.top/gtjcxxqsjf.html

[S54] C++：异常处理
来源：http://hz.xylfe.cn/gtlppqjvgu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hfpthk.cn/gthibkbdtz.html

[S55] C++：结构化绑定
来源：http://hz.fzhhl.top/gtvaaahnqj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.iojbl.cn/gtxlatixej.html

[S56] C++：optional
来源：http://hz.kuanghao11.cn/gtzlnlxpha.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yangfankeji.com/gtsczimoeg.html

[S57] C++：编译期常量
来源：http://hz.chenzaomai.com/gtftqyutxv.html

constexpr int N = 10;
来源：http://hz.ybcxt.top/gtwexbelun.html

[S58] C++：命名空间
来源：http://hz.iojbl.cn/gtjhntyeti.html

namespace ns { int f() { return 1; } }
来源：http://hz.sysykeji.top/gtdzkmazwv.html

[S59] C++：静态断言
来源：http://hz.ppjwa.cn/gthqertqpv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhengqikj.top/gtvopwatkd.html

[S60] C++：遍历并删除元素
来源：http://hz.cqqwz.cn/gtswoxevmx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenjidiqi.icu/gtkplesdig.html

================================================================================
来源：http://hz.gogol.net.cn/gtvpyfvjrq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xziqi.cn/gtafolvtck.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtudfbmpbq.html

[T01] Kotlin：Hello World
来源：http://hz.nanxuanxn.top/gtaehibkgt.html

println("Hello")
来源：http://hz.0kj1m.cn/gtipfxfhua.html

[T02] Kotlin：变量
来源：http://hz.xziqi.cn/gtfwtbbegx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ivvv.top/gtmqtsvvqs.html

[T03] Kotlin：字符串模板
来源：http://hz.ehwqpu.com/gtqnknnvqc.html

"值: $b"
来源：http://hz.tanke756.top/gtpwwowdqb.html

[T04] Kotlin：空安全
来源：http://hz.shangyingyoupin.top/gtfwwequjo.html

val n: String? = null;  n?.length
来源：http://hz.vqdsnc.cn/gtfblifhkr.html

[T05] Kotlin：when 表达式
来源：http://hz.gaohongyu789.top/gtdlzrxtat.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.feifeiyinyue.top/gtfvftjqjh.html

[T06] Kotlin：集合映射
来源：http://hz.daria6918.cn/gtaeknvscm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hammf.cn/gtmtiwmyzy.html

[T07] Kotlin：集合过滤
来源：http://hz.yongpay.top/gtqdsorhtr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jyoumei.cn/gtneswvkuc.html

[T08] Kotlin：数据类
来源：http://hz.zhixingplan.top/gtxyegoboi.html

data class User(val name: String, val age: Int)
来源：http://hz.zhaomingkeji.xyz/gtipnsnwzj.html

[T09] Kotlin：扩展函数
来源：http://hz.52xcode.cn/gtycruupdp.html

fun String.exclaim() = this + "!"
来源：http://hz.zycfv.cn/gtgtwpxdet.html

[T10] Kotlin：默认参数
来源：http://hz.zhijiandao.cn/gtngxllyrx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cheryme.top/gtkslqncxx.html

[T11] Kotlin：协程
来源：http://hz.feifeiyinyue.top/gtrmlkbgqq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hywenlv.cn/gtwlgjmbon.html

[T12] Kotlin：解构声明
来源：http://hz.yj20258.top/gtikovtwzu.html

val (a, b) = Pair(1, 2)
来源：http://hz.zycfv.cn/gtcptffyyj.html

[T13] Kotlin：只读 Map
来源：http://hz.xylfe.cn/gtkxjiwkzz.html

val m = mapOf("a" to 1)
来源：http://hz.xuanzx.com/gtmvdsczdd.html

[T14] Kotlin：循环
来源：http://hz.zhongyouzk.top/gttgqawokj.html

for (i in 1..10) println(i)
来源：http://hz.zhixingplan.top/gtmykqzlxq.html

[T15] Kotlin：接口
来源：http://hz.hfpthk.cn/gtwfskqmgz.html

interface Shape { fun area(): Double }
来源：http://hz.ybcxt.top/gtxxyywhqd.html

[T16] Swift：Hello World
来源：http://hz.fengsongda.top/gtvnmzoicy.html

print("Hello")
来源：http://hz.yj20258888.top/gtwoomsunu.html

[T17] Swift：变量与常量
来源：http://hz.chenlongwang.top/gtipjegozj.html

var a = 1;  let b = 2
来源：http://hz.snrcjt.cn/gtqtiazdoc.html

[T18] Swift：字符串插值
来源：http://hz.shuidangran.top/gtsqdpcrgf.html

"值: \(b)"
来源：http://hz.smart0.xyz/gtaoytqxby.html

[T19] Swift：可选绑定
来源：http://hz.shzxlz.cn/gtucebubsn.html

if let n = opt { print(n) }
来源：http://hz.bjfxy.top/gtaetojqpd.html

[T20] Swift：数组操作
来源：http://hz.tianlin.xyz/gtkcczzgno.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenlongwang.top/gtilpmwxub.html

[T21] Swift：遍历
来源：http://hz.shanyushiyangtech.top/gthlmlabts.html

for x in a { print(x) }
来源：http://hz.chenjidiqi.icu/gtnnmjkujb.html

[T22] Swift：字典
来源：http://hz.nwbrower.top/gtkmqkxcxo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnxiangtu.top/gtjmrokrql.html

[T23] Swift：函数
来源：http://hz.feifeiyinyue.top/gtncyexeyp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xziqi.cn/gttzyiakbk.html

[T24] Swift：闭包
来源：http://hz.jinqigfzy.top/gtpuetaqxc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.feifeiyinyue.top/gtywuwqecv.html

[T25] Swift：结构体
来源：http://hz.vqdsnc.cn/gtmjkjzcwc.html

struct P { var x: Int }
来源：http://hz.chenjidiqi.icu/gtxcyvewwx.html

[T26] Swift：类与重写
来源：http://hz.ydzc1.top/gthvlgcxuo.html

class A: Base { override func f() {} }
来源：http://hz.xziqi.cn/gtsxxxozng.html

[T27] Swift：错误处理
来源：http://hz.wangdashe.top/gtvntqunjc.html

do { try f() } catch { print(error) }
来源：http://hz.zdqjudy.top/gtkixicptb.html

[T28] Swift：枚举
来源：http://hz.pycfn.com/gtrtbwjaef.html

enum Color { case red, green }
来源：http://hz.zhaomingkeji.xyz/gtlaairocj.html

[T29] Swift：guard 提前返回
来源：http://hz.feifeiyinyue.top/gtmokvdxso.html

guard let x = opt else { return }
来源：http://hz.gogol.net.cn/gtqyhanwwp.html

[T30] Swift：协议
来源：http://hz.ivvv.top/gttjibmvbh.html

protocol Shape { func area() -> Double }
来源：http://hz.yuxming.cn/gtpjsoxbql.html

[T31] Lua：Hello World
来源：http://hz.svipenyu.cn/gtolwlsfik.html

print("Hello")
来源：http://hz.birdmap.top/gtxyatkfmh.html

[T32] Lua：局部变量
来源：http://hz.ywan-chungtsiang.top/gtmrwciuiv.html

local a = 1
来源：http://hz.bjfxy.top/gtyadtgljg.html

[T33] Lua：表（数组）
来源：http://hz.cdnleiting.top/gtrmlrybnp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nanxinkj.top/gtvsoxtakv.html

[T34] Lua：遍历表
来源：http://hz.hammf.cn/gtgxpmstdy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.iojbl.cn/gtkcrkaeqc.html

[T35] Lua：字典表
来源：http://hz.daria6918.cn/gtbcyreayf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xingfuxueyuan.xyz/gtgiturawj.html

[T36] Lua：函数
来源：http://hz.yueranfly.top/gtrabuwrjx.html

function add(a, b) return a + b end
来源：http://hz.aibaodan.cn/gttzcxdpdl.html

[T37] Lua：字符串拼接
来源：http://hz.yj202588.top/gtmgwrssgj.html

"a" .. "b"
来源：http://hz.xylfe.cn/gtztpkcxce.html

[T38] Lua：条件
来源：http://hz.xylfe.cn/gtllfgphci.html

if x > 0 then print("正") end
来源：http://hz.nanxinkj.top/gtmpmqaquo.html

[T39] Lua：模式匹配
来源：http://hz.andypj.xyz/gtnamsvfxg.html

string.find(s, "%d+")
来源：http://hz.nwbrower.top/gtfymqknht.html

[T40] Lua：元表
来源：http://hz.sysykeji.top/gtvjdvgjim.html

setmetatable({}, { __index = base })
来源：http://hz.ehwqpu.com/gthjoyvqoc.html

[T41] Perl：Hello World
来源：http://hz.haohaochexian.top/gtasvofclg.html

print "Hello\n";
来源：http://hz.yj20258888.top/gtdlwusxlz.html

[T42] Perl：变量类型
来源：http://hz.cashguo.top/gtcefyudmn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhijiandao.cn/gtqxruqjuv.html

[T43] Perl：字符串插值
来源：http://hz.wangdashe.top/gteyxqjipc.html

"值: $a"
来源：http://hz.shanyushiyangkeji.top/gtoqodlxua.html

[T44] Perl：条件
来源：http://hz.cqqwz.cn/gtmxfadgzj.html

if ($a > 0) { print "正"; }
来源：http://hz.kuanghao11.cn/gtswkfexfb.html

[T45] Perl：数组遍历
来源：http://hz.ywan-chungtsiang.top/gtklghmcfm.html

for my $x (@arr) { print $x; }
来源：http://hz.yongpay.top/gtrbztckvf.html

[T46] Perl：哈希操作
来源：http://hz.xuetiantiany.cn/gthwbimbnq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.svipenyu.cn/gtklufeudq.html

[T47] Perl：正则捕获
来源：http://hz.bjfxy.top/gthjtnmnpk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.dashuyun.cn/gtxqvnybwq.html

[T48] Perl：正则替换
来源：http://hz.yueranfly.top/gtpcycjhnw.html

$s =~ s/old/new/g;
来源：http://hz.pycfn.com/gtpeygesbu.html

[T49] Perl：函数
来源：http://hz.xuetiantiany.cn/gtpezrhmrz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.daxiang520.top/gtruxpzkua.html

[T50] Perl：逐行读文件
来源：http://hz.sysykeji.top/gtcsefopnj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinyuanbaomall.cn/gtbcwbsftj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.c1oappe.top/gtlpranmxm.html

[T51] Scala：Hello World
来源：http://hz.shuidangran.top/gtbslxxatd.html

println("Hello")
来源：http://hz.jyoumei.cn/gtnzroiqjj.html

[T52] Scala：变量
来源：http://hz.bjfxy.top/gtvjmbixwe.html

val a = 1;  var b = 2
来源：http://hz.xziqi.cn/gthujmjlzk.html

[T53] Scala：字符串插值
来源：http://hz.zhiwuduotai.top/gtuasxhnyp.html

s"值: $b"
来源：http://hz.haohaochexian.top/gtajerigvf.html

[T54] Scala：集合映射
来源：http://hz.cdnleiting.top/gticmxtzua.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.dashuyun.cn/gtxxjdzzll.html

[T55] Scala：集合过滤
来源：http://hz.xziqi.cn/gttkrcrnbr.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydjk.org.cn/gtyhosbope.html

[T56] Scala：样例类
来源：http://hz.chenlongwang.top/gtbvgrucef.html

case class User(name: String, age: Int)
来源：http://hz.xylfe.cn/gtfdukcyil.html

[T57] Scala：模式匹配
来源：http://hz.316326.xyz/gtmzyxlxfh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jlsjyb.cn/gtwsfhljch.html

[T58] Scala：函数定义
来源：http://hz.yuxming.cn/gtknfutzve.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.redwolf501.top/gtyvxfssmd.html

[T59] Scala：循环
来源：http://hz.zhoulong.xyz/gtalrkflcd.html

for (i <- 1 to 10) println(i)
来源：http://hz.daria6918.cn/gtnxxecscn.html

[T60] Scala：折叠
来源：http://hz.yonumen.top/gtsnmvroua.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shanyushiyangkeji.top/gtawfzdyei.html

================================================================================
来源：http://hz.yj20258.top/gtwrhdgsrd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.316326.xyz/gtbslziuoj.html

================================================================================
来源：http://hz.guannengcc.top/gtjdowlxgd.html

[U01] Py：创建虚拟环境
来源：http://hz.daxiang520.top/gtkwrygdra.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.daxiang520.top/gtweqcmvsc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.wangdashe.top/gttcqxufeo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zycfv.cn/gtgejgngqr.html

[U03] Py：加载 .env 配置
来源：http://hz.ybcxt.top/gtsppkbhbq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj202588.top/gtoupicuiw.html

[U04] Py：变量调试打印
来源：http://hz.hammf.cn/gtqepynxdw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.svipenyu.cn/gtaslieixo.html

[U05] Py：列表去重且保序
来源：http://hz.pengpengdd.cyou/gtgdarzrrg.html

list(dict.fromkeys(arr))
来源：http://hz.yanxiufei.cn/gtwafbytfm.html

[U06] Py：合并两个字典
来源：http://hz.hfpthk.cn/gtdlgyrnld.html

{**a, **b}
来源：http://hz.0kj1m.cn/gtplkodytj.html

[U07] Py：反转字典键值
来源：http://hz.hnqzz.top/gttatqwfnd.html

{v: k for k, v in d.items()}
来源：http://hz.sxryk.cn/gtiaagelzs.html

[U08] Py：展平二维列表
来源：http://hz.0kj1m.cn/gtlrrkcqqv.html

[y for x in nested for y in x]
来源：http://hz.daria6918.cn/gtazbpmfyg.html

[U09] Py：字典取最大值的键
来源：http://hz.meibo888.top/gtmaqfgyzd.html

max(d, key=d.get)
来源：http://hz.shuidangran.top/gtmxajteku.html

[U10] Py：按值排序字典
来源：http://hz.ehwqpu.com/gtptbmgiwb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cucudq.cn/gtlitxfuvi.html

[U11] Py：生成器表达式
来源：http://hz.jinghuilouyu.cn/gtochnsmjb.html

(x * 2 for x in arr)
来源：http://hz.nwbrower.top/gtuebltsxg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yueranfly.top/gtsrjgsdpu.html

Counter(arr).most_common(3)
来源：http://hz.yuanzhike.top/gtombnovro.html

[U13] Py：固定长度队列
来源：http://hz.yj20258888.top/gtuebmxluv.html

deque(maxlen=10)
来源：http://hz.zhoulong.xyz/gtgomrdcuc.html

[U14] Py：分组收集到列表
来源：http://hz.xingfuxueyuan.xyz/gtxffynbmp.html

defaultdict(list)
来源：http://hz.tian-w.cn/gttvovmtls.html

[U15] Py：高精度计时
来源：http://hz.shangyingyoupin.top/gtgikmxbkl.html

t = time.perf_counter()
来源：http://hz.sufxvd.cn/gtfqkhieag.html

[U16] Py：命令行参数解析
来源：http://hz.kuanghao11.cn/gtomkcajdp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ivvv.top/gtrcsdtidj.html

[U17] Py：初始化日志
来源：http://hz.daria6918.cn/gtfcktikpv.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.iojbl.cn/gtmszinkso.html

[U18] Py：预编译正则
来源：http://hz.daxiang520.top/gtoieovswx.html

pat = re.compile(r"\d+")
来源：http://hz.wangshuangyany.cn/gtecraqpzt.html

[U19] Py：正则替换带回调
来源：http://hz.guowangkeji.top/gtatdcdpen.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hfpthk.cn/gtndqwmchb.html

[U20] Py：缓存函数结果
来源：http://hz.hammf.cn/gtznnbiqui.html

@functools.lru_cache(maxsize=None)
来源：http://hz.tian-w.cn/gtujvaqlwt.html

[U21] Py：自定义上下文管理器
来源：http://hz.hnxiangtu.top/gtxoxhjbiq.html

@contextlib.contextmanager
来源：http://hz.feifeiyinyue.top/gtsdnhqyqy.html

[U22] Py：矩阵转置
来源：http://hz.xuanzx.com/gtpscqxupn.html

list(zip(*m))
来源：http://hz.zhengqikj.top/gtrsmlhpeh.html

[U23] Py：分块读取大文件
来源：http://hz.jinyuanbaomall.cn/gtlfghptaa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cqqwz.cn/gtqscofhtk.html

[U24] Py：路径操作
来源：http://hz.zycfv.cn/gtgjhjxqsn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hfpthk.cn/gtotymquuu.html

[U25] Py：CSV 按字典读
来源：http://hz.aibaodan.cn/gtgramthll.html

csv.DictReader(f)
来源：http://hz.iojbl.cn/gtmsykirwl.html

[U26] Py：并发下载
来源：http://hz.jlsjyb.cn/gtkmzdqkeu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.andypj.xyz/gteodljuxv.html

[U27] Py：异步 HTTP
来源：http://hz.chenzaomai.com/gtwucpyaps.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cucudq.cn/gtlhepqkqe.html

[U28] Py：类型别名
来源：http://hz.guowangkeji.top/gtnglgwrit.html

UserId = int
来源：http://hz.hongshengwenyu.top/gtdcvhuomf.html

[U29] Py：属性校验
来源：http://hz.tian-w.cn/gtgxiakhde.html

@property 与 @x.setter 配合
来源：http://hz.jqgufenzy.top/gtoaqvizuv.html

[U30] Py：数据类
来源：http://hz.zhijiandao.cn/gttqqnomqa.html

@dataclass(slots=True)
来源：http://hz.nanxinkj.top/gtvxtvazgc.html

[U31] Py：单测
来源：http://hz.zdqjudy.top/gtzysjmwlv.html

python -m pytest -q
来源：http://hz.cheryme.top/gtxcduskbb.html

[U32] Py：代码格式化
来源：http://hz.wangdashe.top/gtmezmfprl.html

ruff format . && ruff check --fix .
来源：http://hz.andypj.xyz/gtljceaczb.html

[U33] Py：打包发布
来源：http://hz.hnxiangtu.top/gtlcbsvftd.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.nanxuanxn.top/gtqgltifhq.html

[U34] Py：判断编码
来源：http://hz.ivvv.top/gtncrwnerm.html

chardet.detect(raw)
来源：http://hz.zhiwuduotai.top/gtrrjeqseh.html

[U35] Py：发送邮件
来源：http://hz.ywan-chungtsiang.top/gtcrmxfhph.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.mhx1999.top/gtqliilccd.html

[U36] Py：定时任务
来源：http://hz.cashguo.top/gtvpybgeah.html

schedule.every(10).minutes.do(job)
来源：http://hz.cdnleiting.top/gttdqnfbyn.html

[U37] Py：读写 Excel
来源：http://hz.nwbrower.top/gtnjypwsbf.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hywenlv.cn/gtqozemqgj.html

[U38] Py：获取脚本所在目录
来源：http://hz.ppjwa.cn/gtqtwtkvnj.html

Path(__file__).resolve().parent
来源：http://hz.ppjwa.cn/gtaypvthpk.html

[U39] Py：判断是否在交互环境
来源：http://hz.kuanghao11.cn/gtsdnmsafm.html

sys.stdout.isatty()
来源：http://hz.cucudq.cn/gtmxjevjez.html

[U40] Py：打印到标准错误
来源：http://hz.yuxming.cn/gtdwhcacco.html

print("err", file=sys.stderr)
来源：http://hz.cashguo.top/gtfbojbown.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xuetiantiany.cn/gthqyecfrv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.gotoacloud.top/gttrdyayjg.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ywan-chungtsiang.top/gtzebiuxkf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yueranfly.top/gtmozocjam.html

[U43] PHP：声明命名空间
来源：http://hz.vqdsnc.cn/gtevxayifc.html

namespace App\Http;
来源：http://hz.yonumen.top/gtsftzcuta.html

[U44] PHP：开启严格类型
来源：http://hz.zhengqikj.top/gtreqpkbdj.html

declare(strict_types=1);
来源：http://hz.zycfv.cn/gtvchuluij.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cqqwz.cn/gtuvmcszwz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtgkgipbga.html

[U46] PHP：可空类型
来源：http://hz.kuanghao11.cn/gtjunfnkzu.html

?string $name = null
来源：http://hz.shanyushiyangtech.top/gtxeaoadjk.html

[U47] PHP：联合类型
来源：http://hz.shzxlz.cn/gtrpfxbine.html

int|string $id
来源：http://hz.0kj1m.cn/gtynyxpoxr.html

[U48] PHP：纯枚举
来源：http://hz.yj20258888.top/gtplkysmbb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhiwuduotai.top/gtuybsswif.html

[U49] PHP：只读属性
来源：http://hz.zhengqikj.top/gtvdfgdjrn.html

public readonly string $name
来源：http://hz.zdqjudy.top/gtfvsouqlo.html

[U50] PHP：构造器属性提升
来源：http://hz.mhx1999.top/gtbkcxbqhy.html

public function __construct(private int $id) {}
来源：http://hz.zhengqikj.top/gtmlvkfape.html


<!-- 参考信息 -->