代发 wailian999

static int counter = 0;
来源：http://hz.tanke756.top/gtijejotnc.html

[S29] C：变参函数
来源：http://hz.hongshengwenyu.top/gtkwlnosji.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhixingplan.top/gtubkyukfl.html

[S30] C：头文件保护
来源：http://hz.yj20258888.top/gtetzjwvoj.html

#ifndef X_H
来源：http://hz.guowangkeji.top/gtzmlsvhtw.html

#define X_H
来源：http://hz.iojbl.cn/gtgpbrxyix.html

#endif
来源：http://hz.fengsongda.top/gtrwuaibob.html

[S31] C++：Hello World
来源：http://hz.zhaomingkeji.xyz/gtkigottex.html

#include <iostream>
来源：http://hz.ybcxt.top/gtxzjccdxl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.guowangkeji.top/gtzxqoskno.html

[S32] C++：字符串
来源：http://hz.ivvv.top/gtubxqkmhr.html

std::string s = "hi";  s += "!";
来源：http://hz.c1oappe.top/gtdbtselux.html

[S33] C++：vector 增删
来源：http://hz.nwbrower.top/gtsfdsfqmb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.iojbl.cn/gteihcbnod.html

[S34] C++：遍历 vector
来源：http://hz.xziqi.cn/gthsxubced.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhoulong.xyz/gtgpcehlht.html

[S35] C++：map
来源：http://hz.ppjwa.cn/gtevpvjmua.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aizwys.cn/gtdghonyxj.html

[S36] C++：unordered_map
来源：http://hz.smart0.xyz/gttletptuy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gogol.net.cn/gthunbehpm.html

[S37] C++：set
来源：http://hz.c1oappe.top/gtmxsavbyc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hongshengwenyu.top/gtumqesmxm.html

[S38] C++：排序
来源：http://hz.aibaodan.cn/gtxagwcaas.html

std::sort(v.begin(), v.end());
来源：http://hz.iojbl.cn/gtwktapkvy.html

[S39] C++：自定义比较器排序
来源：http://hz.birdmap.top/gttfraemkn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ppjwa.cn/gtfaowewxe.html

[S40] C++：查找元素
来源：http://hz.hfpthk.cn/gtrshsnqrp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xuetiantiany.cn/gtctphhgab.html

[S41] C++：类与构造函数
来源：http://hz.zhijiandao.cn/gtnfdwvhzc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.guannengcc.top/gtfqjjttlr.html

[S42] C++：继承与虚函数
来源：http://hz.fengsongda.top/gtnrisydcm.html

class B : public Base { public: void f() override {} };
来源：http://hz.52xcode.cn/gtxosgawku.html

[S43] C++：智能指针
来源：http://hz.zhixingplan.top/gtcxyjvvcb.html

auto p = std::make_unique<int>(5);
来源：http://hz.bjfxy.top/gtjtoovqpk.html

[S44] C++：引用传参
来源：http://hz.aizwys.cn/gtrfpridqb.html

void inc(int &x) { ++x; }
来源：http://hz.jqgfzy.top/gtjhqgchok.html

[S45] C++：lambda
来源：http://hz.zhixingplan.top/gtktznwjaq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gzhubu.top/gtcsimqoop.html

[S46] C++：函数模板
来源：http://hz.xuanzx.com/gthhhzwera.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yueranfly.top/gtdsmoelim.html

[S47] C++：结构化绑定遍历
来源：http://hz.shanyushiyangkeji.top/gtayuqzsvq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hysaishi.cn/gtgzchlacz.html

[S48] C++：逐行读文件
来源：http://hz.fengsongda.top/gtxgadxxmw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtgzzdwvoi.html

while (std::getline(in, line)) { }
来源：http://hz.ehwqpu.com/gtfochhfvh.html

[S49] C++：写文件
来源：http://hz.zhijiandao.cn/gtlmkqlxia.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ehwqpu.com/gtvryghdht.html

[S50] C++：格式化数字
来源：http://hz.guannengcc.top/gtecftaupy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cqqwz.cn/gtsvodaees.html

[S51] C++：显式类型转换
来源：http://hz.pycfn.com/gtqcxfwdvh.html

static_cast<double>(a) / b
来源：http://hz.mhx1999.top/gtnertrotz.html

[S52] C++：const 与 noexcept
来源：http://hz.zhijiandao.cn/gtbmurcuvx.html

int size() const noexcept { return n_; }
来源：http://hz.nanxuanxn.top/gtkyvvgzfl.html

[S53] C++：移动语义
来源：http://hz.svipenyu.cn/gtxoifozno.html

std::vector<int> w = std::move(v);
来源：http://hz.vqdsnc.cn/gtsajcctbd.html

[S54] C++：异常处理
来源：http://hz.jianghu66.top/gthuhxufcf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hongshengwenyu.top/gtbpyiotjy.html

[S55] C++：结构化绑定
来源：http://hz.bjfxy.top/gtmwvgjwpp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cdnleiting.top/gttalohyzp.html

[S56] C++：optional
来源：http://hz.gzhubu.top/gtavvrhtwu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cdnleiting.top/gtbqlyrwyy.html

[S57] C++：编译期常量
来源：http://hz.yj20258.top/gtixmvxohp.html

constexpr int N = 10;
来源：http://hz.shangyingyoupin.top/gtndqqnsnh.html

[S58] C++：命名空间
来源：http://hz.tian-w.cn/gtcaxqtlye.html

namespace ns { int f() { return 1; } }
来源：http://hz.nwbrower.top/gtusymbtbt.html

[S59] C++：静态断言
来源：http://hz.pengpengdd.cyou/gtiwpuselj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenjidiqi.icu/gtplabrmus.html

[S60] C++：遍历并删除元素
来源：http://hz.snrcjt.cn/gtdajezqem.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.quarkkingdee.top/gthhviwmah.html

================================================================================
来源：http://hz.snrcjt.cn/gtwvvoutyh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daxiang520.top/gtanqjhybd.html

================================================================================
来源：http://hz.yueranfly.top/gtcgfmzxpc.html

[T01] Kotlin：Hello World
来源：http://hz.smart0.xyz/gtiwstvalh.html

println("Hello")
来源：http://hz.fzhhl.top/gtunvxhxdm.html

[T02] Kotlin：变量
来源：http://hz.smart0.xyz/gthdtypprr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xziqi.cn/gtatcyiknz.html

[T03] Kotlin：字符串模板
来源：http://hz.cashguo.top/gtejyjznbf.html

"值: $b"
来源：http://hz.gogol.net.cn/gtetslcpqq.html

[T04] Kotlin：空安全
来源：http://hz.snrcjt.cn/gttovcuupl.html

val n: String? = null;  n?.length
来源：http://hz.shzxlz.cn/gtxoslgfdf.html

[T05] Kotlin：when 表达式
来源：http://hz.hongshengwenyu.top/gtsprrqqjt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.pengpengdd.cyou/gtotjbwirl.html

[T06] Kotlin：集合映射
来源：http://hz.andypj.xyz/gtgxipugum.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.52xcode.cn/gtnsyippmk.html

[T07] Kotlin：集合过滤
来源：http://hz.jlsjyb.cn/gtjsvvszxi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zdqjudy.top/gtwucgghjs.html

[T08] Kotlin：数据类
来源：http://hz.ppjwa.cn/gttrclstjj.html

data class User(val name: String, val age: Int)
来源：http://hz.redwolf501.top/gtxvbmhdfi.html

[T09] Kotlin：扩展函数
来源：http://hz.smart0.xyz/gtdilpdzqp.html

fun String.exclaim() = this + "!"
来源：http://hz.svipenyu.cn/gtqizvvwlv.html

[T10] Kotlin：默认参数
来源：http://hz.daxiang520.top/gtqcmhmziy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgufenzy.top/gtxypytqof.html

[T11] Kotlin：协程
来源：http://hz.hnqzz.top/gttoyblrfl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.52xcode.cn/gtvxcbwsbv.html

[T12] Kotlin：解构声明
来源：http://hz.yuanzhike.top/gtncmnjvit.html

val (a, b) = Pair(1, 2)
来源：http://hz.pycfn.com/gttlzisetp.html

[T13] Kotlin：只读 Map
来源：http://hz.hongshengwenyu.top/gtlbsqcrqh.html

val m = mapOf("a" to 1)
来源：http://hz.yueranfly.top/gtlixfzxkv.html

[T14] Kotlin：循环
来源：http://hz.zdqjudy.top/gtzfwoiahp.html

for (i in 1..10) println(i)
来源：http://hz.meibo888.top/gtiaewbvxu.html

[T15] Kotlin：接口
来源：http://hz.fengsongda.top/gtgopeqbal.html

interface Shape { fun area(): Double }
来源：http://hz.vqdsnc.cn/gtrmudieed.html

[T16] Swift：Hello World
来源：http://hz.yj202588.top/gttyijmsqr.html

print("Hello")
来源：http://hz.bjfxy.top/gtlngnneor.html

[T17] Swift：变量与常量
来源：http://hz.yonumen.top/gtlesvodcu.html

var a = 1;  let b = 2
来源：http://hz.xylfe.cn/gtxcradwng.html

[T18] Swift：字符串插值
来源：http://hz.ydzc1.top/gtrwuxwaak.html

"值: \(b)"
来源：http://hz.ivvv.top/gtphjvjruk.html

[T19] Swift：可选绑定
来源：http://hz.yuanzhike.top/gtiisilikz.html

if let n = opt { print(n) }
来源：http://hz.quarkkingdee.top/gtaduvzqmf.html

[T20] Swift：数组操作
来源：http://hz.dashuyun.cn/gtfbjfljfo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shangyingyoupin.top/gtpkkmmplc.html

[T21] Swift：遍历
来源：http://hz.aibaodan.cn/gtnyhcljje.html

for x in a { print(x) }
来源：http://hz.nanxuanxn.top/gtdewtojae.html

[T22] Swift：字典
来源：http://hz.yongpay.top/gtkynhhblg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhaomingkeji.xyz/gtfwgtbfnn.html

[T23] Swift：函数
来源：http://hz.bjfxy.top/gtgflqssrg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yangfankeji.com/gtfntjrjra.html

[T24] Swift：闭包
来源：http://hz.52xcode.cn/gtpjitmhnc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.svipenyu.cn/gtvhemngio.html

[T25] Swift：结构体
来源：http://hz.yj20258888.top/gtndwcmwxz.html

struct P { var x: Int }
来源：http://hz.zdqjudy.top/gtsvtdornm.html

[T26] Swift：类与重写
来源：http://hz.9152youxi.cn/gtbxkzxlbe.html

class A: Base { override func f() {} }
来源：http://hz.ydjk.org.cn/gtmkanbvvx.html

[T27] Swift：错误处理
来源：http://hz.ydzc1.top/gtepmvkhil.html

do { try f() } catch { print(error) }
来源：http://hz.dashuyun.cn/gtsnxgwlxp.html

[T28] Swift：枚举
来源：http://hz.jlsjyb.cn/gtkijrnbbr.html

enum Color { case red, green }
来源：http://hz.hywenlv.cn/gtcgpbonxu.html

[T29] Swift：guard 提前返回
来源：http://hz.yanxiufei.cn/gteqsgvkmh.html

guard let x = opt else { return }
来源：http://hz.tianlin.xyz/gtvuqeszqz.html

[T30] Swift：协议
来源：http://hz.gogol.net.cn/gtekkjfnys.html

protocol Shape { func area() -> Double }
来源：http://hz.tanke756.top/gtbqjbwvvc.html

[T31] Lua：Hello World
来源：http://hz.snrcjt.cn/gtgkmvcbhd.html

print("Hello")
来源：http://hz.hnxiangtu.top/gtnraaehvc.html

[T32] Lua：局部变量
来源：http://hz.guannengcc.top/gtwqrxjdkj.html

local a = 1
来源：http://hz.hywenlv.cn/gtndiepmbi.html

[T33] Lua：表（数组）
来源：http://hz.sysykeji.top/gtncouctvs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.guowangkeji.top/gtxerdfwhx.html

[T34] Lua：遍历表
来源：http://hz.sysykeji.top/gtqeikzfkq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.guowangkeji.top/gtbidoceaj.html

[T35] Lua：字典表
来源：http://hz.feifeiyinyue.top/gtxvcqawzi.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shanyushiyangkeji.top/gtbmowlcmp.html

[T36] Lua：函数
来源：http://hz.zhengqikj.top/gtqqmcsbgf.html

function add(a, b) return a + b end
来源：http://hz.gotoacloud.top/gtdnidpyzy.html

[T37] Lua：字符串拼接
来源：http://hz.ppjwa.cn/gtbwchztcy.html

"a" .. "b"
来源：http://hz.hammf.cn/gtmdtkibav.html

[T38] Lua：条件
来源：http://hz.0kj1m.cn/gtyvmcsrkq.html

if x > 0 then print("正") end
来源：http://hz.yvedp.cn/gtapswvcpe.html

[T39] Lua：模式匹配
来源：http://hz.xingfuxueyuan.xyz/gtdfzckijb.html

string.find(s, "%d+")
来源：http://hz.iojbl.cn/gtcmvjxfhg.html

[T40] Lua：元表
来源：http://hz.chenjidiqi.icu/gtaycagcon.html

setmetatable({}, { __index = base })
来源：http://hz.bjfxy.top/gtzoevuvum.html

[T41] Perl：Hello World
来源：http://hz.316326.xyz/gtmoafizmb.html

print "Hello\n";
来源：http://hz.jqgufenzy.top/gtvpbmobfy.html

[T42] Perl：变量类型
来源：http://hz.ybcxt.top/gtrlmtnswr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinghuilouyu.cn/gtleyjmcjx.html

[T43] Perl：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtcjmhflwy.html

"值: $a"
来源：http://hz.guannengcc.top/gtumbhnqjk.html

[T44] Perl：条件
来源：http://hz.pengpengdd.cyou/gtjbgclggb.html

if ($a > 0) { print "正"; }
来源：http://hz.nanxuanxn.top/gtwbchddoi.html

[T45] Perl：数组遍历
来源：http://hz.c1oappe.top/gtzllulueo.html

for my $x (@arr) { print $x; }
来源：http://hz.yangfankeji.com/gtmawbzmdc.html

[T46] Perl：哈希操作
来源：http://hz.cheryme.top/gtnkammjom.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.chenzaomai.com/gtzoitvufy.html

[T47] Perl：正则捕获
来源：http://hz.shzxlz.cn/gtmicqlgrr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.kuanghao11.cn/gtkefmfcxz.html

[T48] Perl：正则替换
来源：http://hz.zhengqikj.top/gtgzitownd.html

$s =~ s/old/new/g;
来源：http://hz.yanxiufei.cn/gtghszjpuq.html

[T49] Perl：函数
来源：http://hz.yvedp.cn/gtqbdbrjlk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.quarkkingdee.top/gtitvhnncr.html

[T50] Perl：逐行读文件
来源：http://hz.0kj1m.cn/gtsnzjgssk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ydjk.org.cn/gtpjjyjbtf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shuidangran.top/gthvhvxcgs.html

[T51] Scala：Hello World
来源：http://hz.pycfn.com/gthvcnqlob.html

println("Hello")
来源：http://hz.gotoacloud.top/gtusqqoexb.html

[T52] Scala：变量
来源：http://hz.sxryk.cn/gtxrwribur.html

val a = 1;  var b = 2
来源：http://hz.redwolf501.top/gtvbrbrsfe.html

[T53] Scala：字符串插值
来源：http://hz.yangfankeji.com/gtwzqchgao.html

s"值: $b"
来源：http://hz.zhongyouzk.top/gtnikzinvm.html

[T54] Scala：集合映射
来源：http://hz.chenzaomai.com/gtidwvaviy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xuetiantiany.cn/gtmzknpaxf.html

[T55] Scala：集合过滤
来源：http://hz.sysykeji.top/gtfexxrgwj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sxryk.cn/gtmwrztwut.html

[T56] Scala：样例类
来源：http://hz.zhoulong.xyz/gtaxmnupxc.html

case class User(name: String, age: Int)
来源：http://hz.gogol.net.cn/gtmgbrqcmt.html

[T57] Scala：模式匹配
来源：http://hz.dianchejie.cn/gthafcdakd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yangfankeji.com/gtxhqidksx.html

[T58] Scala：函数定义
来源：http://hz.hywenlv.cn/gtkrwkolsl.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cucudq.cn/gthybhokxl.html

[T59] Scala：循环
来源：http://hz.tian-w.cn/gttjlezvre.html

for (i <- 1 to 10) println(i)
来源：http://hz.shuidangran.top/gttsxrxoij.html

[T60] Scala：折叠
来源：http://hz.guannengcc.top/gtelrsmnmi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhengqikj.top/gtqugvnpmi.html

================================================================================
来源：http://hz.aibaodan.cn/gtbiotvgpg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.pengpengdd.cyou/gtdrbmzkyc.html

================================================================================
来源：http://hz.ybcxt.top/gtarteitip.html

[U01] Py：创建虚拟环境
来源：http://hz.gotoacloud.top/gtqfopscaj.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.pengpengdd.cyou/gtaondbqwq.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jqgufenzy.top/gtreqnxllz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.dashuyun.cn/gtkjuiquki.html

[U03] Py：加载 .env 配置
来源：http://hz.cucudq.cn/gtkpnpqask.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hnxiangtu.top/gtcvdxsovm.html

[U04] Py：变量调试打印
来源：http://hz.ehwqpu.com/gtfyufgtrd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhijiandao.cn/gtqbzpzgfn.html

[U05] Py：列表去重且保序
来源：http://hz.jiagoushi.top/gtrhcrglee.html

list(dict.fromkeys(arr))
来源：http://hz.pycfn.com/gtzkwrontv.html

[U06] Py：合并两个字典
来源：http://hz.c1oappe.top/gtqwsmybks.html

{**a, **b}
来源：http://hz.hnqzz.top/gtmoaiwcnz.html

[U07] Py：反转字典键值
来源：http://hz.shuidangran.top/gtnyyzvwao.html

{v: k for k, v in d.items()}
来源：http://hz.gzhubu.top/gtxlxuyvuq.html

[U08] Py：展平二维列表
来源：http://hz.wangdashe.top/gtgqiucuuf.html

[y for x in nested for y in x]
来源：http://hz.haohaochexian.top/gtdeksvips.html

[U09] Py：字典取最大值的键
来源：http://hz.fzhhl.top/gtnqwegwer.html

max(d, key=d.get)
来源：http://hz.ydjk.org.cn/gtsqbqpdat.html

[U10] Py：按值排序字典
来源：http://hz.hongshengwenyu.top/gtvhcxxfwa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dashuyun.cn/gtqoguwnhn.html

[U11] Py：生成器表达式
来源：http://hz.pycfn.com/gtwdrpbngp.html

(x * 2 for x in arr)
来源：http://hz.wangdashe.top/gtaaatdhxq.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.vqdsnc.cn/gtxianejrm.html

Counter(arr).most_common(3)
来源：http://hz.aizwys.cn/gtezvlgtre.html

[U13] Py：固定长度队列
来源：http://hz.hfpthk.cn/gtggdyhvht.html

deque(maxlen=10)
来源：http://hz.mhx1999.top/gthkruymrv.html

[U14] Py：分组收集到列表
来源：http://hz.yueranfly.top/gtmlfsrjvm.html

defaultdict(list)
来源：http://hz.vqdsnc.cn/gtndzvgonf.html

[U15] Py：高精度计时
来源：http://hz.zhixingplan.top/gtecqwkbcd.html

t = time.perf_counter()
来源：http://hz.cqqwz.cn/gtfficlvub.html

[U16] Py：命令行参数解析
来源：http://hz.svipenyu.cn/gtdvmfdrzp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.tian-w.cn/gtsghzrscg.html

[U17] Py：初始化日志
来源：http://hz.xylfe.cn/gtqvxcuzqf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.tanke756.top/gtexhcqmxf.html

[U18] Py：预编译正则
来源：http://hz.zhijiandao.cn/gtwvrbmsyx.html

pat = re.compile(r"\d+")
来源：http://hz.gogol.net.cn/gtbqfiixcf.html

[U19] Py：正则替换带回调
来源：http://hz.fzhhl.top/gtotuxgrny.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jinqigfzy.top/gtpolyrfde.html

[U20] Py：缓存函数结果
来源：http://hz.shangyingyoupin.top/gtydzsvfns.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xylfe.cn/gtvopudsmu.html

[U21] Py：自定义上下文管理器
来源：http://hz.jqgfzy.top/gteiblyjos.html

@contextlib.contextmanager
来源：http://hz.havefunace.top/gtvjssrcyn.html

[U22] Py：矩阵转置
来源：http://hz.pycfn.com/gtwtvkfgqt.html

list(zip(*m))
来源：http://hz.hongshengwenyu.top/gtzdrlasbf.html

[U23] Py：分块读取大文件
来源：http://hz.guowangkeji.top/gtcvzvoceo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cheryme.top/gtsnbgtyrz.html

[U24] Py：路径操作
来源：http://hz.shanyushiyangkeji.top/gtkvfcctpu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yongpay.top/gteszlemnj.html

[U25] Py：CSV 按字典读
来源：http://hz.cheryme.top/gtwnefobgg.html

csv.DictReader(f)
来源：http://hz.tianlin.xyz/gtmkmktops.html

[U26] Py：并发下载
来源：http://hz.feifeiyinyue.top/gtqzzpmcbr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.guannengcc.top/gtnemgsvjq.html

[U27] Py：异步 HTTP
来源：http://hz.nanxuanxn.top/gtsfjtxhot.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ppjwa.cn/gtcxvkwvju.html

[U28] Py：类型别名
来源：http://hz.xinyue.icu/gtgsfxnmxl.html

UserId = int
来源：http://hz.ppjwa.cn/gthmaaiyyc.html

[U29] Py：属性校验
来源：http://hz.tianlin.xyz/gtcszzljwy.html

@property 与 @x.setter 配合
来源：http://hz.guowangkeji.top/gtsowoxphy.html

[U30] Py：数据类
来源：http://hz.9152youxi.cn/gtuxgapubr.html

@dataclass(slots=True)
来源：http://hz.ivvv.top/gthhecmtws.html

[U31] Py：单测
来源：http://hz.shangyingyoupin.top/gtefduamqt.html

python -m pytest -q
来源：http://hz.sufxvd.cn/gtyzrdbwqw.html

[U32] Py：代码格式化
来源：http://hz.xuanzx.com/gtwxwahtjp.html

ruff format . && ruff check --fix .
来源：http://hz.shuidangran.top/gtcguserpz.html

[U33] Py：打包发布
来源：http://hz.chenlongwang.top/gtjpbcidiw.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shzxlz.cn/gthtmaqhyg.html

[U34] Py：判断编码
来源：http://hz.hongshengwenyu.top/gtwztaapmp.html

chardet.detect(raw)
来源：http://hz.zhaomingkeji.xyz/gturjhephx.html

[U35] Py：发送邮件
来源：http://hz.tian-w.cn/gtosaopycs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yj20258.top/gtwxfwlkrp.html

[U36] Py：定时任务
来源：http://hz.zhoulong.xyz/gtanhjyojq.html

schedule.every(10).minutes.do(job)
来源：http://hz.9152youxi.cn/gtuqlagckf.html

[U37] Py：读写 Excel
来源：http://hz.chenlongwang.top/gttbquszpp.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ehwqpu.com/gtcnsahzca.html

[U38] Py：获取脚本所在目录
来源：http://hz.xylfe.cn/gtzxsquude.html

Path(__file__).resolve().parent
来源：http://hz.jinghuilouyu.cn/gtobmzcaao.html

[U39] Py：判断是否在交互环境
来源：http://hz.52xcode.cn/gtzbnbkjed.html

sys.stdout.isatty()
来源：http://hz.bjfxy.top/gtvedovsru.html

[U40] Py：打印到标准错误
来源：http://hz.shanyushiyangtech.top/gtrmbdlldq.html

print("err", file=sys.stderr)
来源：http://hz.nanxuanxn.top/gtzoyaifbl.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zdqjudy.top/gtcnxouann.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.fzhhl.top/gtjmbjjkhg.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gaohongyu789.top/gtpyfjiypd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.haohaochexian.top/gtjahevstm.html

[U43] PHP：声明命名空间
来源：http://hz.fengsongda.top/gttucsfxaf.html

namespace App\Http;
来源：http://hz.xylfe.cn/gtzbmeymac.html

[U44] PHP：开启严格类型
来源：http://hz.jyoumei.cn/gthnbuibzv.html

declare(strict_types=1);
来源：http://hz.shuidangran.top/gtlpxqyylb.html

[U45] PHP：类型声明与返回类型
来源：http://hz.daxiang520.top/gtxskxclww.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtvnwnntuf.html

[U46] PHP：可空类型
来源：http://hz.zhiwuduotai.top/gtwqmwyxxx.html

?string $name = null
来源：http://hz.vqdsnc.cn/gtmcabyizk.html

[U47] PHP：联合类型
来源：http://hz.hywenlv.cn/gtplsdskeg.html

int|string $id
来源：http://hz.yongpay.top/gtluiblfod.html

[U48] PHP：纯枚举
来源：http://hz.zhaomingkeji.xyz/gtqbadmwqy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.bjfxy.top/gtgtejxxrh.html

[U49] PHP：只读属性
来源：http://hz.guowangkeji.top/gttmustbzp.html

public readonly string $name
来源：http://hz.jianghu66.top/gtqfvstvaw.html

[U50] PHP：构造器属性提升
来源：http://hz.daxiang520.top/gtwtzbdtbx.html

public function __construct(private int $id) {}
来源：http://hz.gogol.net.cn/gtjvncmzfk.html

[U51] PHP：数组解构
来源：http://hz.cashguo.top/gtvxqfsiqh.html

[$a, $b] = $arr;
来源：http://hz.yj20258888.top/gtidymbivk.html

[U52] PHP：箭头函数
来源：http://hz.0kj1m.cn/gtbcuhsgtu.html

$double = fn($x) => $x * 2;
来源：http://hz.jqgfzy.top/gtxrpxmlmf.html


<!-- 参考信息 -->