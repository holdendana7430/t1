代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhaomingkeji.xyz/gtrgntlgtk.html

[S25] C：内存拷贝
来源：http://hz.zhiwuduotai.top/gtxcgffzak.html

memcpy(dst, src, n);
来源：http://hz.jianghu66.top/gtdvohnckl.html

[S26] C：内存清零
来源：http://hz.gotoacloud.top/gtqlkplznr.html

memset(a, 0, sizeof a);
来源：http://hz.andypj.xyz/gtkukerzbh.html

[S27] C：定义常量
来源：http://hz.yanxiufei.cn/gtunqimius.html

const double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtomwugvuy.html

[S28] C：静态变量
来源：http://hz.jinyuanbaomall.cn/gtrhkuglfx.html

static int counter = 0;
来源：http://hz.xingfuxueyuan.xyz/gtlncrhper.html

[S29] C：变参函数
来源：http://hz.ehwqpu.com/gthbeidyuz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.vqdsnc.cn/gtsaognddm.html

[S30] C：头文件保护
来源：http://hz.sxryk.cn/gtrqenzfwi.html

#ifndef X_H
来源：http://hz.yj202588.top/gtrfpzkobb.html

#define X_H
来源：http://hz.cheryme.top/gtkalzohfw.html

#endif
来源：http://hz.ybcxt.top/gtxorjktbj.html

[S31] C++：Hello World
来源：http://hz.cqqwz.cn/gtqkakukgb.html

#include <iostream>
来源：http://hz.cashguo.top/gtyqybdmdd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.smart0.xyz/gthqvtfabb.html

[S32] C++：字符串
来源：http://hz.nanxuanxn.top/gtaqrbwdry.html

std::string s = "hi";  s += "!";
来源：http://hz.havefunace.top/gtmjqsxkti.html

[S33] C++：vector 增删
来源：http://hz.316326.xyz/gtjjolgbzb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yonumen.top/gtvmqdsjil.html

[S34] C++：遍历 vector
来源：http://hz.0kj1m.cn/gtheiyhnzm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nanxinkj.top/gtfomnrdnv.html

[S35] C++：map
来源：http://hz.feifeiyinyue.top/gtucacqsji.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtldrvyqlk.html

[S36] C++：unordered_map
来源：http://hz.cdnleiting.top/gtwpecjslj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258.top/gtoagsmmvb.html

[S37] C++：set
来源：http://hz.ppjwa.cn/gttddkwzet.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jlsjyb.cn/gtajwwwtpm.html

[S38] C++：排序
来源：http://hz.mhx1999.top/gtqthiftfd.html

std::sort(v.begin(), v.end());
来源：http://hz.havefunace.top/gtlgykdenw.html

[S39] C++：自定义比较器排序
来源：http://hz.andypj.xyz/gtxyrulscw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.vqdsnc.cn/gtdpndonho.html

[S40] C++：查找元素
来源：http://hz.wangdashe.top/gtavayuwjh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhaomingkeji.xyz/gtzrsahcae.html

[S41] C++：类与构造函数
来源：http://hz.c1oappe.top/gtmwusivxc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zdqjudy.top/gtvnypssnk.html

[S42] C++：继承与虚函数
来源：http://hz.pycfn.com/gtcgoqfjqn.html

class B : public Base { public: void f() override {} };
来源：http://hz.vqdsnc.cn/gtgjfnrqki.html

[S43] C++：智能指针
来源：http://hz.52xcode.cn/gtwdnmdpee.html

auto p = std::make_unique<int>(5);
来源：http://hz.shuidangran.top/gtmiqdinvr.html

[S44] C++：引用传参
来源：http://hz.nwbrower.top/gtwznxxswy.html

void inc(int &x) { ++x; }
来源：http://hz.zhaomingkeji.xyz/gtfvwwsypo.html

[S45] C++：lambda
来源：http://hz.wangdashe.top/gtpyexqvdn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.feifeiyinyue.top/gtbyjrpehs.html

[S46] C++：函数模板
来源：http://hz.shzxlz.cn/gtsfgsyekf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnxiangtu.top/gtwbogqnln.html

[S47] C++：结构化绑定遍历
来源：http://hz.guannengcc.top/gtekndtvnb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.c1oappe.top/gthwdfvgci.html

[S48] C++：逐行读文件
来源：http://hz.9152youxi.cn/gtzlpnxbdc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangtech.top/gtiphxzwou.html

while (std::getline(in, line)) { }
来源：http://hz.cheryme.top/gtlvemkfyv.html

[S49] C++：写文件
来源：http://hz.bjfxy.top/gtoqeflnwz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cqqwz.cn/gtdqsnouzl.html

[S50] C++：格式化数字
来源：http://hz.zhoulong.xyz/gtnxmauvjv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.havefunace.top/gtrqwyadub.html

[S51] C++：显式类型转换
来源：http://hz.zhoulong.xyz/gtsshavhci.html

static_cast<double>(a) / b
来源：http://hz.tanke756.top/gtevmzyqao.html

[S52] C++：const 与 noexcept
来源：http://hz.zhoulong.xyz/gtskijzfiq.html

int size() const noexcept { return n_; }
来源：http://hz.feifeiyinyue.top/gtqjphsxls.html

[S53] C++：移动语义
来源：http://hz.dianchejie.cn/gtymsdzuof.html

std::vector<int> w = std::move(v);
来源：http://hz.jinyuanbaomall.cn/gtnibrrqsc.html

[S54] C++：异常处理
来源：http://hz.cashguo.top/gtvrfcvrze.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgufenzy.top/gtuktqwoke.html

[S55] C++：结构化绑定
来源：http://hz.meibo888.top/gtzsmfjubq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xylfe.cn/gtdzivhdcr.html

[S56] C++：optional
来源：http://hz.zhiwuduotai.top/gtoeoyjfmx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shanyushiyangtech.top/gtzmclppxl.html

[S57] C++：编译期常量
来源：http://hz.sxryk.cn/gtryojpcgo.html

constexpr int N = 10;
来源：http://hz.ydjk.org.cn/gtlvdywxqo.html

[S58] C++：命名空间
来源：http://hz.316326.xyz/gtzcgsbley.html

namespace ns { int f() { return 1; } }
来源：http://hz.shanyushiyangtech.top/gtqnxjwtyq.html

[S59] C++：静态断言
来源：http://hz.bjfxy.top/gtbpktteyv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj20258.top/gtdqaupuuu.html

[S60] C++：遍历并删除元素
来源：http://hz.zdqjudy.top/gthwnyxgxa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhijiandao.cn/gtswyucwao.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtkfvfpnkx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.vqdsnc.cn/gtqmywgrgt.html

================================================================================
来源：http://hz.gotoacloud.top/gtbeizmvzn.html

[T01] Kotlin：Hello World
来源：http://hz.gzhubu.top/gttsuztcds.html

println("Hello")
来源：http://hz.cqqwz.cn/gtxgzmhuci.html

[T02] Kotlin：变量
来源：http://hz.jianghu66.top/gtezthcgea.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.guannengcc.top/gtrdskklqg.html

[T03] Kotlin：字符串模板
来源：http://hz.cucudq.cn/gtvxnvvdai.html

"值: $b"
来源：http://hz.ydjk.org.cn/gtffgqgnon.html

[T04] Kotlin：空安全
来源：http://hz.tanke756.top/gtwggfaecd.html

val n: String? = null;  n?.length
来源：http://hz.jianghu66.top/gtyiovnxpa.html

[T05] Kotlin：when 表达式
来源：http://hz.zhiwuduotai.top/gttplepcor.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhixingplan.top/gtrmhzfvsw.html

[T06] Kotlin：集合映射
来源：http://hz.xziqi.cn/gtulrcdqfy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zdqjudy.top/gtlthedwwb.html

[T07] Kotlin：集合过滤
来源：http://hz.chenzaomai.com/gtxdtgmxso.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gzhubu.top/gtmwbfhhmv.html

[T08] Kotlin：数据类
来源：http://hz.haohaochexian.top/gtmvrocbqk.html

data class User(val name: String, val age: Int)
来源：http://hz.havefunace.top/gtxrxovgpw.html

[T09] Kotlin：扩展函数
来源：http://hz.wangdashe.top/gtlivuqfrm.html

fun String.exclaim() = this + "!"
来源：http://hz.gzhubu.top/gtszznntyf.html

[T10] Kotlin：默认参数
来源：http://hz.nanxinkj.top/gtwffhaezq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daria6918.cn/gtbtgvvrqj.html

[T11] Kotlin：协程
来源：http://hz.ivvv.top/gtklmzxhwj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gaohongyu789.top/gthkcsvtns.html

[T12] Kotlin：解构声明
来源：http://hz.sufxvd.cn/gtulxnoofq.html

val (a, b) = Pair(1, 2)
来源：http://hz.316326.xyz/gtbfjseknh.html

[T13] Kotlin：只读 Map
来源：http://hz.jqgufenzy.top/gtjyvsngfu.html

val m = mapOf("a" to 1)
来源：http://hz.zhoulong.xyz/gtercpwcrq.html

[T14] Kotlin：循环
来源：http://hz.shanyushiyangkeji.top/gtvmpjiiae.html

for (i in 1..10) println(i)
来源：http://hz.tanke756.top/gtblfacnko.html

[T15] Kotlin：接口
来源：http://hz.tianlin.xyz/gtapeuhtkj.html

interface Shape { fun area(): Double }
来源：http://hz.birdmap.top/gtehpjxkug.html

[T16] Swift：Hello World
来源：http://hz.xziqi.cn/gtcdxkyobr.html

print("Hello")
来源：http://hz.jinqigfzy.top/gtblfxnznn.html

[T17] Swift：变量与常量
来源：http://hz.jlsjyb.cn/gtbnetknfi.html

var a = 1;  let b = 2
来源：http://hz.xuetiantiany.cn/gtbacawdyj.html

[T18] Swift：字符串插值
来源：http://hz.yj20258888.top/gtfidqqwzr.html

"值: \(b)"
来源：http://hz.cqqwz.cn/gtdlhqtpzd.html

[T19] Swift：可选绑定
来源：http://hz.chenzaomai.com/gtgaedecmp.html

if let n = opt { print(n) }
来源：http://hz.daxiang520.top/gtpsltuznw.html

[T20] Swift：数组操作
来源：http://hz.nanxinkj.top/gtwofrwcgx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cashguo.top/gtoxoptozz.html

[T21] Swift：遍历
来源：http://hz.yongpay.top/gtxhkiyeev.html

for x in a { print(x) }
来源：http://hz.tanke756.top/gtfoootyix.html

[T22] Swift：字典
来源：http://hz.yvedp.cn/gtounlwjsr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinghuilouyu.cn/gtwdmutakb.html

[T23] Swift：函数
来源：http://hz.guannengcc.top/gtvaecjulr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhengqikj.top/gtpseftyxr.html

[T24] Swift：闭包
来源：http://hz.zhoulong.xyz/gtvlksafcl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.9152youxi.cn/gtszkmmhwr.html

[T25] Swift：结构体
来源：http://hz.guowangkeji.top/gtxhbivjik.html

struct P { var x: Int }
来源：http://hz.shanyushiyangkeji.top/gtothizlfg.html

[T26] Swift：类与重写
来源：http://hz.gaohongyu789.top/gteyhlbkvs.html

class A: Base { override func f() {} }
来源：http://hz.xuanzx.com/gtsstxxosa.html

[T27] Swift：错误处理
来源：http://hz.jinqigufen.top/gtzaitnfbt.html

do { try f() } catch { print(error) }
来源：http://hz.hfpthk.cn/gtvdcvbeyx.html

[T28] Swift：枚举
来源：http://hz.zycfv.cn/gtjmajgegt.html

enum Color { case red, green }
来源：http://hz.xingfuxueyuan.xyz/gtwbnimbxz.html

[T29] Swift：guard 提前返回
来源：http://hz.xylfe.cn/gtisbothem.html

guard let x = opt else { return }
来源：http://hz.zycfv.cn/gteskxolyx.html

[T30] Swift：协议
来源：http://hz.hnxiangtu.top/gteodryglf.html

protocol Shape { func area() -> Double }
来源：http://hz.guannengcc.top/gtcwrgdhxl.html

[T31] Lua：Hello World
来源：http://hz.hysaishi.cn/gtocselpti.html

print("Hello")
来源：http://hz.yj20258.top/gtdpswhmfd.html

[T32] Lua：局部变量
来源：http://hz.gzhubu.top/gtwjomyuks.html

local a = 1
来源：http://hz.jqgfzy.top/gtbelgoljr.html

[T33] Lua：表（数组）
来源：http://hz.yongpay.top/gtkzqkqvlc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hnxiangtu.top/gtkiypbnrg.html

[T34] Lua：遍历表
来源：http://hz.haohaochexian.top/gtrvniunxg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tianlin.xyz/gtewrrfkly.html

[T35] Lua：字典表
来源：http://hz.snrcjt.cn/gtcttfuwrj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gotoacloud.top/gthcueyjnw.html

[T36] Lua：函数
来源：http://hz.aizwys.cn/gtgaxfnlom.html

function add(a, b) return a + b end
来源：http://hz.gogol.net.cn/gtqvvohxbx.html

[T37] Lua：字符串拼接
来源：http://hz.xingfuxueyuan.xyz/gthngqeddu.html

"a" .. "b"
来源：http://hz.jianghu66.top/gtwsigymyr.html

[T38] Lua：条件
来源：http://hz.zhijiandao.cn/gthlwpvffv.html

if x > 0 then print("正") end
来源：http://hz.zhiwuduotai.top/gtgvmjvqmg.html

[T39] Lua：模式匹配
来源：http://hz.zdqjudy.top/gtrrpnsixp.html

string.find(s, "%d+")
来源：http://hz.guannengcc.top/gtrudctokb.html

[T40] Lua：元表
来源：http://hz.ybcxt.top/gtuiyltmgq.html

setmetatable({}, { __index = base })
来源：http://hz.316326.xyz/gtjfmowbfo.html

[T41] Perl：Hello World
来源：http://hz.hywenlv.cn/gtysysdwpl.html

print "Hello\n";
来源：http://hz.ydjk.org.cn/gtzjlczzfm.html

[T42] Perl：变量类型
来源：http://hz.ivvv.top/gtgauqucpz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shanyushiyangtech.top/gtvjtdtmls.html

[T43] Perl：字符串插值
来源：http://hz.zycfv.cn/gttetuylrw.html

"值: $a"
来源：http://hz.ivvv.top/gtpiofrqmq.html

[T44] Perl：条件
来源：http://hz.shanyushiyangkeji.top/gtuxkxehpb.html

if ($a > 0) { print "正"; }
来源：http://hz.jinghuilouyu.cn/gtvnvubgjh.html

[T45] Perl：数组遍历
来源：http://hz.zhongyouzk.top/gthfwoapyd.html

for my $x (@arr) { print $x; }
来源：http://hz.daria6918.cn/gtjzohtgfn.html

[T46] Perl：哈希操作
来源：http://hz.daria6918.cn/gtrqdquisj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258.top/gtfzlwdzjo.html

[T47] Perl：正则捕获
来源：http://hz.tian-w.cn/gthgelufce.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinqigfzy.top/gtcouedcsk.html

[T48] Perl：正则替换
来源：http://hz.guannengcc.top/gtkadbdtzf.html

$s =~ s/old/new/g;
来源：http://hz.redwolf501.top/gtpkygcrgd.html

[T49] Perl：函数
来源：http://hz.jinqigfzy.top/gtcdxheumo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhongyouzk.top/gtkhlxthim.html

[T50] Perl：逐行读文件
来源：http://hz.guannengcc.top/gtytonyhrp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zdqjudy.top/gthoqzhoab.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ywan-chungtsiang.top/gtegwexfva.html

[T51] Scala：Hello World
来源：http://hz.jinyuanbaomall.cn/gtpldrxkyo.html

println("Hello")
来源：http://hz.316326.xyz/gttwzyhisl.html

[T52] Scala：变量
来源：http://hz.jinqigfzy.top/gtfvqcskze.html

val a = 1;  var b = 2
来源：http://hz.havefunace.top/gtoewhclht.html

[T53] Scala：字符串插值
来源：http://hz.chenjidiqi.icu/gtvemsedxc.html

s"值: $b"
来源：http://hz.guannengcc.top/gtblzwcljc.html

[T54] Scala：集合映射
来源：http://hz.jinqigufen.top/gtimeghrzm.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.iojbl.cn/gtzqprcrtm.html

[T55] Scala：集合过滤
来源：http://hz.jinqigfzy.top/gtidpfxfek.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhaomingkeji.xyz/gtlvknlpfl.html

[T56] Scala：样例类
来源：http://hz.shanyushiyangtech.top/gtijnbiakh.html

case class User(name: String, age: Int)
来源：http://hz.jyoumei.cn/gtebvymlkc.html

[T57] Scala：模式匹配
来源：http://hz.sufxvd.cn/gtruwhcxiv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.andypj.xyz/gtajgrgtdo.html

[T58] Scala：函数定义
来源：http://hz.sweek.top/gtvunxqrdu.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xinyue.icu/gttghcvzuf.html

[T59] Scala：循环
来源：http://hz.c1oappe.top/gtkjdtqnxs.html

for (i <- 1 to 10) println(i)
来源：http://hz.mhx1999.top/gtbeyhzjda.html

[T60] Scala：折叠
来源：http://hz.pycfn.com/gtmqxahxub.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shangyingyoupin.top/gtjcihzdus.html

================================================================================
来源：http://hz.jiagoushi.top/gtmnbfdiei.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.wangdashe.top/gtseaefqyy.html

================================================================================
来源：http://hz.hfpthk.cn/gtvacvszil.html

[U01] Py：创建虚拟环境
来源：http://hz.dianchejie.cn/gtoqdytiin.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ydjk.org.cn/gteuhwaxiz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.vqdsnc.cn/gtxropddzr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.pycfn.com/gtbbojkgwy.html

[U03] Py：加载 .env 配置
来源：http://hz.pycfn.com/gtlkqdpefl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhongyouzk.top/gtffceibfe.html

[U04] Py：变量调试打印
来源：http://hz.xuetiantiany.cn/gtywkrijrj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yuxming.cn/gtmokyivlh.html

[U05] Py：列表去重且保序
来源：http://hz.daxiang520.top/gtkxcjzzrf.html

list(dict.fromkeys(arr))
来源：http://hz.haohaochexian.top/gthcxshzqi.html

[U06] Py：合并两个字典
来源：http://hz.zycfv.cn/gtorslajth.html

{**a, **b}
来源：http://hz.yvedp.cn/gtnobtbnrz.html

[U07] Py：反转字典键值
来源：http://hz.andypj.xyz/gtojcefeiv.html

{v: k for k, v in d.items()}
来源：http://hz.c1oappe.top/gtosxrqrzd.html

[U08] Py：展平二维列表
来源：http://hz.zhijiandao.cn/gtnhgubtbr.html

[y for x in nested for y in x]
来源：http://hz.daria6918.cn/gtxfrtalow.html

[U09] Py：字典取最大值的键
来源：http://hz.jianghu66.top/gtavxeggsm.html

max(d, key=d.get)
来源：http://hz.jyoumei.cn/gtbovtpmlb.html

[U10] Py：按值排序字典
来源：http://hz.hnqzz.top/gtadgrpdad.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xuetiantiany.cn/gtbntyslse.html

[U11] Py：生成器表达式
来源：http://hz.0kj1m.cn/gtiybezcmq.html

(x * 2 for x in arr)
来源：http://hz.gzhubu.top/gtogfcmflc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.52xcode.cn/gtdhshotet.html

Counter(arr).most_common(3)
来源：http://hz.c1oappe.top/gtpjueckfn.html

[U13] Py：固定长度队列
来源：http://hz.hnqzz.top/gtgfpiynya.html

deque(maxlen=10)
来源：http://hz.hammf.cn/gteqwffbhl.html

[U14] Py：分组收集到列表
来源：http://hz.wangshuangyany.cn/gtunmoxmch.html

defaultdict(list)
来源：http://hz.ydjk.org.cn/gtwqbshyve.html

[U15] Py：高精度计时
来源：http://hz.ybcxt.top/gtlqlephht.html

t = time.perf_counter()
来源：http://hz.jqgufenzy.top/gtvgrogzia.html

[U16] Py：命令行参数解析
来源：http://hz.iojbl.cn/gtfzggpqxl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.52xcode.cn/gtbrgmeybj.html

[U17] Py：初始化日志
来源：http://hz.redwolf501.top/gtctiqdzbs.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jianghu66.top/gtkysgyjdm.html

[U18] Py：预编译正则
来源：http://hz.hammf.cn/gtfgyhedll.html

pat = re.compile(r"\d+")
来源：http://hz.zhengqikj.top/gtsvpwemgp.html

[U19] Py：正则替换带回调
来源：http://hz.iojbl.cn/gtywiojrrp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shuidangran.top/gtqndeyjcx.html

[U20] Py：缓存函数结果
来源：http://hz.sweek.top/gtbherdzzb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj202588.top/gtmuugbyuy.html

[U21] Py：自定义上下文管理器
来源：http://hz.birdmap.top/gtbbxgxnmm.html

@contextlib.contextmanager
来源：http://hz.ppjwa.cn/gtrjufwncz.html

[U22] Py：矩阵转置
来源：http://hz.shangyingyoupin.top/gtjqfmajsz.html

list(zip(*m))
来源：http://hz.xinyue.icu/gtocnlukfp.html

[U23] Py：分块读取大文件
来源：http://hz.shanyushiyangkeji.top/gtefczdgrf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ydjk.org.cn/gtnhwjqwdp.html

[U24] Py：路径操作
来源：http://hz.316326.xyz/gtmfnrvqhq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.nanxinkj.top/gtkwtegaui.html

[U25] Py：CSV 按字典读
来源：http://hz.meibo888.top/gtqyvwqwhn.html

csv.DictReader(f)
来源：http://hz.ydzc1.top/gtptooojwc.html

[U26] Py：并发下载
来源：http://hz.chenjidiqi.icu/gtpjhimjcc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yuxming.cn/gtizbdisrr.html

[U27] Py：异步 HTTP
来源：http://hz.sweek.top/gtvreospiw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.mhx1999.top/gtmwnhnykj.html

[U28] Py：类型别名
来源：http://hz.birdmap.top/gtacexeiwi.html

UserId = int
来源：http://hz.cashguo.top/gtrkwenpge.html

[U29] Py：属性校验
来源：http://hz.shuidangran.top/gtivmjyzmp.html

@property 与 @x.setter 配合
来源：http://hz.xziqi.cn/gthfehziin.html

[U30] Py：数据类
来源：http://hz.sysykeji.top/gtctnqooyt.html

@dataclass(slots=True)
来源：http://hz.hysaishi.cn/gtapvmlsng.html

[U31] Py：单测
来源：http://hz.gogol.net.cn/gtpxuykzur.html

python -m pytest -q
来源：http://hz.aizwys.cn/gtqtnaphnf.html

[U32] Py：代码格式化
来源：http://hz.shzxlz.cn/gtubmanzgy.html

ruff format . && ruff check --fix .
来源：http://hz.hnxiangtu.top/gtdrpwlpsc.html

[U33] Py：打包发布
来源：http://hz.yj202588.top/gtufyrayxa.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yj20258.top/gtsufopzai.html

[U34] Py：判断编码
来源：http://hz.9152youxi.cn/gtmwxzduuw.html

chardet.detect(raw)
来源：http://hz.yangfankeji.com/gthjtlwfhu.html

[U35] Py：发送邮件
来源：http://hz.tanke756.top/gtxdegnfee.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nanxinkj.top/gtpjhxfloa.html

[U36] Py：定时任务
来源：http://hz.sxryk.cn/gtkcykuxvk.html

schedule.every(10).minutes.do(job)
来源：http://hz.cdnleiting.top/gtehsfnqrk.html

[U37] Py：读写 Excel
来源：http://hz.guowangkeji.top/gtogkyblls.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shangyingyoupin.top/gtpndaoexk.html

[U38] Py：获取脚本所在目录
来源：http://hz.andypj.xyz/gttdyunwih.html

Path(__file__).resolve().parent
来源：http://hz.yueranfly.top/gtoqozcvjv.html

[U39] Py：判断是否在交互环境
来源：http://hz.redwolf501.top/gtkgqnmjzg.html

sys.stdout.isatty()
来源：http://hz.zdqjudy.top/gtsffgjwhv.html

[U40] Py：打印到标准错误
来源：http://hz.shanyushiyangkeji.top/gtzaksfqaa.html

print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtwnbjwcpr.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhoulong.xyz/gtstsxpgtz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.nanxuanxn.top/gttvwhrfqc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhaomingkeji.xyz/gtrmgsmrcz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xuanzx.com/gtnuvuexog.html

[U43] PHP：声明命名空间
来源：http://hz.shzxlz.cn/gteayhwium.html

namespace App\Http;
来源：http://hz.zhoulong.xyz/gtyfchvhiv.html

[U44] PHP：开启严格类型
来源：http://hz.c1oappe.top/gtryajhdca.html

declare(strict_types=1);
来源：http://hz.hammf.cn/gtvnnsthxi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhijiandao.cn/gtximjlzup.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtrkwjbjfk.html

[U46] PHP：可空类型
来源：http://hz.aizwys.cn/gtvwmwyzuw.html

?string $name = null
来源：http://hz.jinqigfzy.top/gtxjblcxpx.html

[U47] PHP：联合类型
来源：http://hz.shzxlz.cn/gtaptteviz.html

int|string $id
来源：http://hz.ppjwa.cn/gtxralkmze.html

[U48] PHP：纯枚举
来源：http://hz.c1oappe.top/gtqhdovfvv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hfpthk.cn/gtrkqmlcfa.html


<!-- 参考信息 -->