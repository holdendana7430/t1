代发 wailian999

memset(a, 0, sizeof a);
来源：http://hz.hongshengwenyu.top/gtbtsyzynj.html

[S27] C：定义常量
来源：http://hz.cashguo.top/gtldztwcco.html

const double PI = 3.14159;
来源：http://hz.ppjwa.cn/gtkvrzyzqu.html

[S28] C：静态变量
来源：http://hz.meibo888.top/gtdnysuwxn.html

static int counter = 0;
来源：http://hz.redwolf501.top/gtszrignti.html

[S29] C：变参函数
来源：http://hz.xylfe.cn/gtqfhxhlpx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zycfv.cn/gtpzwymamv.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangkeji.top/gtywcalzya.html

#ifndef X_H
来源：http://hz.tian-w.cn/gtjdhryagb.html

#define X_H
来源：http://hz.andypj.xyz/gtnliorbjr.html

#endif
来源：http://hz.0kj1m.cn/gtfyoqlshr.html

[S31] C++：Hello World
来源：http://hz.shzxlz.cn/gtbyjjpnou.html

#include <iostream>
来源：http://hz.haohaochexian.top/gtjlytqpxg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ydjk.org.cn/gtespxptig.html

[S32] C++：字符串
来源：http://hz.ehwqpu.com/gttgaajvgf.html

std::string s = "hi";  s += "!";
来源：http://hz.yj202588.top/gtlymjpmhj.html

[S33] C++：vector 增删
来源：http://hz.meibo888.top/gthyfnhois.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinqigfzy.top/gtukkzxezf.html

[S34] C++：遍历 vector
来源：http://hz.ybcxt.top/gtsbqwblcu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cucudq.cn/gtfiizilwv.html

[S35] C++：map
来源：http://hz.yuanzhike.top/gtvfyiblnk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gtvtxmevrh.html

[S36] C++：unordered_map
来源：http://hz.shanyushiyangkeji.top/gtpjxgzaan.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ywan-chungtsiang.top/gttisotjmg.html

[S37] C++：set
来源：http://hz.xinyue.icu/gtmwkqbppa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xingfuxueyuan.xyz/gtxxsqpbpi.html

[S38] C++：排序
来源：http://hz.zhongyouzk.top/gtxypmhuog.html

std::sort(v.begin(), v.end());
来源：http://hz.ivvv.top/gtxugafskn.html

[S39] C++：自定义比较器排序
来源：http://hz.yonumen.top/gtrqaljpln.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxinkj.top/gtgdcnbmpo.html

[S40] C++：查找元素
来源：http://hz.wangshuangyany.cn/gtqypjdozy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxinkj.top/gtsccjsluu.html

[S41] C++：类与构造函数
来源：http://hz.bjfxy.top/gtrtqovnov.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yangfankeji.com/gtlubouwwa.html

[S42] C++：继承与虚函数
来源：http://hz.nwbrower.top/gtbvkmseno.html

class B : public Base { public: void f() override {} };
来源：http://hz.hammf.cn/gttgogasox.html

[S43] C++：智能指针
来源：http://hz.sweek.top/gtqnndmucq.html

auto p = std::make_unique<int>(5);
来源：http://hz.daxiang520.top/gtqvrdjiik.html

[S44] C++：引用传参
来源：http://hz.jyoumei.cn/gthyfjyyss.html

void inc(int &x) { ++x; }
来源：http://hz.jyoumei.cn/gtzhubshem.html

[S45] C++：lambda
来源：http://hz.zhoulong.xyz/gttnpfjaww.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shuidangran.top/gtugdcemwf.html

[S46] C++：函数模板
来源：http://hz.ybcxt.top/gtrnfvmncn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhaomingkeji.xyz/gtmdahxftq.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenjidiqi.icu/gtjbtolsxt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gogol.net.cn/gtsmhmavgh.html

[S48] C++：逐行读文件
来源：http://hz.daxiang520.top/gtgvggzudw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinghuilouyu.cn/gtazxxovuw.html

while (std::getline(in, line)) { }
来源：http://hz.birdmap.top/gtxhvpnobh.html

[S49] C++：写文件
来源：http://hz.mhx1999.top/gtngsrzvbe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.bjfxy.top/gtnjwugfuy.html

[S50] C++：格式化数字
来源：http://hz.mhx1999.top/gtjmjwowmx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ydzc1.top/gtifbltcuq.html

[S51] C++：显式类型转换
来源：http://hz.zhaomingkeji.xyz/gtopeztezk.html

static_cast<double>(a) / b
来源：http://hz.smart0.xyz/gtmepsssro.html

[S52] C++：const 与 noexcept
来源：http://hz.yangfankeji.com/gtlwcfkzkt.html

int size() const noexcept { return n_; }
来源：http://hz.gogol.net.cn/gtinfyyjcn.html

[S53] C++：移动语义
来源：http://hz.aibaodan.cn/gtremeklkk.html

std::vector<int> w = std::move(v);
来源：http://hz.quarkkingdee.top/gtpbweshal.html

[S54] C++：异常处理
来源：http://hz.jinghuilouyu.cn/gtjhqfckkp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ydzc1.top/gtfavybmue.html

[S55] C++：结构化绑定
来源：http://hz.gaohongyu789.top/gtsahjlnye.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.vqdsnc.cn/gtcgsfpbjl.html

[S56] C++：optional
来源：http://hz.chenzaomai.com/gtruyjkcmy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.iojbl.cn/gtfnrxxqhk.html

[S57] C++：编译期常量
来源：http://hz.snrcjt.cn/gtwirzsioo.html

constexpr int N = 10;
来源：http://hz.wangdashe.top/gtraklnfqk.html

[S58] C++：命名空间
来源：http://hz.jinghuilouyu.cn/gtiggyumjo.html

namespace ns { int f() { return 1; } }
来源：http://hz.redwolf501.top/gtezmwbfmf.html

[S59] C++：静态断言
来源：http://hz.316326.xyz/gtwhcgqdes.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tianlin.xyz/gttszvakom.html

[S60] C++：遍历并删除元素
来源：http://hz.sxryk.cn/gtdyafnqaq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.9152youxi.cn/gtspxgmcln.html

================================================================================
来源：http://hz.cashguo.top/gthitoocjm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuxming.cn/gtxjolobij.html

================================================================================
来源：http://hz.guowangkeji.top/gtblaafhbn.html

[T01] Kotlin：Hello World
来源：http://hz.jyoumei.cn/gtrlnbmsck.html

println("Hello")
来源：http://hz.haohaochexian.top/gtzqagrjjg.html

[T02] Kotlin：变量
来源：http://hz.yangfankeji.com/gtvgczbxwf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangdashe.top/gtxdtxgqwu.html

[T03] Kotlin：字符串模板
来源：http://hz.vqdsnc.cn/gtqslkeuhy.html

"值: $b"
来源：http://hz.zhaomingkeji.xyz/gtiqqaxzer.html

[T04] Kotlin：空安全
来源：http://hz.jinqigfzy.top/gtokrsusmz.html

val n: String? = null;  n?.length
来源：http://hz.gotoacloud.top/gtvngmqiti.html

[T05] Kotlin：when 表达式
来源：http://hz.shangyingyoupin.top/gtbopgyygy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.nanxinkj.top/gteanljanl.html

[T06] Kotlin：集合映射
来源：http://hz.xylfe.cn/gtxahpzjma.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hfpthk.cn/gtdtteeaqg.html

[T07] Kotlin：集合过滤
来源：http://hz.52xcode.cn/gtaztrapvl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.kuanghao11.cn/gtdlzzbazq.html

[T08] Kotlin：数据类
来源：http://hz.316326.xyz/gtcwylucto.html

data class User(val name: String, val age: Int)
来源：http://hz.yongpay.top/gtvwfcblxl.html

[T09] Kotlin：扩展函数
来源：http://hz.chenlongwang.top/gtrlukpixp.html

fun String.exclaim() = this + "!"
来源：http://hz.jinyuanbaomall.cn/gtidvqqxgr.html

[T10] Kotlin：默认参数
来源：http://hz.yanxiufei.cn/gteqaddshg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenzaomai.com/gtfkupvzux.html

[T11] Kotlin：协程
来源：http://hz.xinyue.icu/gtwtalzzbp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.9152youxi.cn/gtvqzjuczl.html

[T12] Kotlin：解构声明
来源：http://hz.ywan-chungtsiang.top/gtgucksaik.html

val (a, b) = Pair(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtxdgvbxol.html

[T13] Kotlin：只读 Map
来源：http://hz.tanke756.top/gtacrjfkcm.html

val m = mapOf("a" to 1)
来源：http://hz.sweek.top/gtmdufclkk.html

[T14] Kotlin：循环
来源：http://hz.yongpay.top/gtksmzjimf.html

for (i in 1..10) println(i)
来源：http://hz.haohaochexian.top/gtlckdzfsj.html

[T15] Kotlin：接口
来源：http://hz.xziqi.cn/gtrzbsaxxi.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gtqegzvjdt.html

[T16] Swift：Hello World
来源：http://hz.fzhhl.top/gtggbsoguj.html

print("Hello")
来源：http://hz.9152youxi.cn/gtgamwsvhf.html

[T17] Swift：变量与常量
来源：http://hz.feifeiyinyue.top/gtslszemat.html

var a = 1;  let b = 2
来源：http://hz.sweek.top/gtuoabifdm.html

[T18] Swift：字符串插值
来源：http://hz.meibo888.top/gthlzfdkec.html

"值: \(b)"
来源：http://hz.dianchejie.cn/gttkjaucda.html

[T19] Swift：可选绑定
来源：http://hz.jinqigfzy.top/gtyerpgyaf.html

if let n = opt { print(n) }
来源：http://hz.hnxiangtu.top/gtulqhmbyo.html

[T20] Swift：数组操作
来源：http://hz.yuxming.cn/gtyxaiiljz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cheryme.top/gtdgmmtmdg.html

[T21] Swift：遍历
来源：http://hz.quarkkingdee.top/gtrqrvlznl.html

for x in a { print(x) }
来源：http://hz.daxiang520.top/gtsrdrfhox.html

[T22] Swift：字典
来源：http://hz.aibaodan.cn/gtadcmgqqh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.52xcode.cn/gtahxiiqxr.html

[T23] Swift：函数
来源：http://hz.chenlongwang.top/gtonflckyw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.316326.xyz/gtdnjwieds.html

[T24] Swift：闭包
来源：http://hz.jyoumei.cn/gtohxnyafj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jyoumei.cn/gtngtcreey.html

[T25] Swift：结构体
来源：http://hz.aizwys.cn/gtepvaodhc.html

struct P { var x: Int }
来源：http://hz.nanxinkj.top/gtqpbizuvq.html

[T26] Swift：类与重写
来源：http://hz.ywan-chungtsiang.top/gtkethvkdk.html

class A: Base { override func f() {} }
来源：http://hz.nanxuanxn.top/gtkjlczriw.html

[T27] Swift：错误处理
来源：http://hz.shuidangran.top/gtngcjtcem.html

do { try f() } catch { print(error) }
来源：http://hz.nanxinkj.top/gtjeuicybb.html

[T28] Swift：枚举
来源：http://hz.sufxvd.cn/gtetiaqhzh.html

enum Color { case red, green }
来源：http://hz.yj202588.top/gtkboxagym.html

[T29] Swift：guard 提前返回
来源：http://hz.jlsjyb.cn/gtwdkvzqrr.html

guard let x = opt else { return }
来源：http://hz.gaohongyu789.top/gtffbuehvk.html

[T30] Swift：协议
来源：http://hz.jqgufenzy.top/gtqgaxhoji.html

protocol Shape { func area() -> Double }
来源：http://hz.dashuyun.cn/gteetmwxts.html

[T31] Lua：Hello World
来源：http://hz.zhoulong.xyz/gthmwlvrby.html

print("Hello")
来源：http://hz.jqgufenzy.top/gtowdfcgar.html

[T32] Lua：局部变量
来源：http://hz.xingfuxueyuan.xyz/gtjiznfayc.html

local a = 1
来源：http://hz.zhaomingkeji.xyz/gtztcstmfg.html

[T33] Lua：表（数组）
来源：http://hz.sweek.top/gtqnpgnlrn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cucudq.cn/gtfyitwojy.html

[T34] Lua：遍历表
来源：http://hz.shzxlz.cn/gturhmlguk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenlongwang.top/gtxarskigv.html

[T35] Lua：字典表
来源：http://hz.xylfe.cn/gtqiaedzsz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.iojbl.cn/gtzefeuvys.html

[T36] Lua：函数
来源：http://hz.yongpay.top/gtdulcqrkg.html

function add(a, b) return a + b end
来源：http://hz.yj20258888.top/gtvtqkepsq.html

[T37] Lua：字符串拼接
来源：http://hz.ydjk.org.cn/gtkeleixnp.html

"a" .. "b"
来源：http://hz.tianlin.xyz/gtritnavqe.html

[T38] Lua：条件
来源：http://hz.feifeiyinyue.top/gtlyizepxm.html

if x > 0 then print("正") end
来源：http://hz.zhijiandao.cn/gtzxmtrkjv.html

[T39] Lua：模式匹配
来源：http://hz.zycfv.cn/gtaefyfbnu.html

string.find(s, "%d+")
来源：http://hz.zhiwuduotai.top/gtnctpkive.html

[T40] Lua：元表
来源：http://hz.ppjwa.cn/gttqjzwmvx.html

setmetatable({}, { __index = base })
来源：http://hz.316326.xyz/gtpumkswoa.html

[T41] Perl：Hello World
来源：http://hz.cucudq.cn/gtektrmqsd.html

print "Hello\n";
来源：http://hz.9152youxi.cn/gttpxseybm.html

[T42] Perl：变量类型
来源：http://hz.yj202588.top/gtbcftkwlr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.c1oappe.top/gthiigrttp.html

[T43] Perl：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gthcnzfwth.html

"值: $a"
来源：http://hz.guannengcc.top/gtldxqmelz.html

[T44] Perl：条件
来源：http://hz.yangfankeji.com/gtskjzpffn.html

if ($a > 0) { print "正"; }
来源：http://hz.meibo888.top/gtckskkzdd.html

[T45] Perl：数组遍历
来源：http://hz.snrcjt.cn/gtmqlgnxbc.html

for my $x (@arr) { print $x; }
来源：http://hz.guowangkeji.top/gtwdiswrxx.html

[T46] Perl：哈希操作
来源：http://hz.52xcode.cn/gtwjhyisrv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ehwqpu.com/gtlkmldrqg.html

[T47] Perl：正则捕获
来源：http://hz.nanxinkj.top/gtlcblmvzy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gotoacloud.top/gtcqmtokhm.html

[T48] Perl：正则替换
来源：http://hz.52xcode.cn/gtiubvyhnq.html

$s =~ s/old/new/g;
来源：http://hz.jyoumei.cn/gtcipeuchi.html

[T49] Perl：函数
来源：http://hz.yj20258.top/gtvkddwykw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenzaomai.com/gtumlvikgj.html

[T50] Perl：逐行读文件
来源：http://hz.gogol.net.cn/gtfpuispsf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zdqjudy.top/gtrlgprfot.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hammf.cn/gtnodzevog.html

[T51] Scala：Hello World
来源：http://hz.sufxvd.cn/gtzleldfbu.html

println("Hello")
来源：http://hz.nwbrower.top/gtizkxxkso.html

[T52] Scala：变量
来源：http://hz.xziqi.cn/gtrbmxvzgt.html

val a = 1;  var b = 2
来源：http://hz.tianlin.xyz/gtvtjozcbx.html

[T53] Scala：字符串插值
来源：http://hz.daria6918.cn/gtygyvexrw.html

s"值: $b"
来源：http://hz.shangyingyoupin.top/gtaykharss.html

[T54] Scala：集合映射
来源：http://hz.bjfxy.top/gtpgzrntkp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.wangshuangyany.cn/gtbtneebev.html

[T55] Scala：集合过滤
来源：http://hz.tian-w.cn/gtczlmbhri.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ywan-chungtsiang.top/gtiqluzhwx.html

[T56] Scala：样例类
来源：http://hz.jinyuanbaomall.cn/gtlykqunli.html

case class User(name: String, age: Int)
来源：http://hz.jiagoushi.top/gtbyyysqva.html

[T57] Scala：模式匹配
来源：http://hz.birdmap.top/gtquvosmvw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gotoacloud.top/gtbjdyirby.html

[T58] Scala：函数定义
来源：http://hz.guowangkeji.top/gthxhuiknm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yanxiufei.cn/gtdsdvhhky.html

[T59] Scala：循环
来源：http://hz.xingfuxueyuan.xyz/gtjgxosqzu.html

for (i <- 1 to 10) println(i)
来源：http://hz.yueranfly.top/gtwqlujrxk.html

[T60] Scala：折叠
来源：http://hz.aibaodan.cn/gtmalqcipx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinqigufen.top/gtytiueksr.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtkipfassp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.pengpengdd.cyou/gtpycinyqz.html

================================================================================
来源：http://hz.hnxiangtu.top/gtvacwspkp.html

[U01] Py：创建虚拟环境
来源：http://hz.yueranfly.top/gtqhqaqboz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tanke756.top/gtdqotprol.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fzhhl.top/gtnyjzvhpp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yj202588.top/gtylhisnyf.html

[U03] Py：加载 .env 配置
来源：http://hz.chenlongwang.top/gtgrqtgser.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ydzc1.top/gtquncnecg.html

[U04] Py：变量调试打印
来源：http://hz.jianghu66.top/gtsaybeyjy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hywenlv.cn/gtihsxbmle.html

[U05] Py：列表去重且保序
来源：http://hz.jyoumei.cn/gtltundzbt.html

list(dict.fromkeys(arr))
来源：http://hz.yongpay.top/gtlzktozcc.html

[U06] Py：合并两个字典
来源：http://hz.tianlin.xyz/gtafbplryw.html

{**a, **b}
来源：http://hz.52xcode.cn/gtfxwdjmba.html

[U07] Py：反转字典键值
来源：http://hz.guowangkeji.top/gtphlvkzro.html

{v: k for k, v in d.items()}
来源：http://hz.yanxiufei.cn/gtqsaayenn.html

[U08] Py：展平二维列表
来源：http://hz.pycfn.com/gtomevswqw.html

[y for x in nested for y in x]
来源：http://hz.chenzaomai.com/gtrxxxnjrp.html

[U09] Py：字典取最大值的键
来源：http://hz.jlsjyb.cn/gtqxqzcayx.html

max(d, key=d.get)
来源：http://hz.tanke756.top/gtgyyogzmt.html

[U10] Py：按值排序字典
来源：http://hz.hnqzz.top/gtdlbefkqn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhijiandao.cn/gtzfuafyzf.html

[U11] Py：生成器表达式
来源：http://hz.0kj1m.cn/gtfnxxhadp.html

(x * 2 for x in arr)
来源：http://hz.birdmap.top/gtkfoagbdu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinqigfzy.top/gtzddrvxws.html

Counter(arr).most_common(3)
来源：http://hz.yuanzhike.top/gtlikgqxod.html

[U13] Py：固定长度队列
来源：http://hz.nanxinkj.top/gtlwwtgayo.html

deque(maxlen=10)
来源：http://hz.aizwys.cn/gtgpouvedn.html

[U14] Py：分组收集到列表
来源：http://hz.snrcjt.cn/gtbivsfewy.html

defaultdict(list)
来源：http://hz.jinqigfzy.top/gtzoujfvqh.html

[U15] Py：高精度计时
来源：http://hz.nanxuanxn.top/gtkgdrspwj.html

t = time.perf_counter()
来源：http://hz.hnxiangtu.top/gtcnkynmca.html

[U16] Py：命令行参数解析
来源：http://hz.jinyuanbaomall.cn/gtnelargdm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.daxiang520.top/gtlttyvgkz.html

[U17] Py：初始化日志
来源：http://hz.iojbl.cn/gteowdkdqo.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.andypj.xyz/gtbbpyczlx.html

[U18] Py：预编译正则
来源：http://hz.ivvv.top/gttlfruslv.html

pat = re.compile(r"\d+")
来源：http://hz.jinghuilouyu.cn/gteiyszfwq.html

[U19] Py：正则替换带回调
来源：http://hz.jinqigfzy.top/gtstkxucmd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.nanxuanxn.top/gtvhpknxvg.html

[U20] Py：缓存函数结果
来源：http://hz.jqgfzy.top/gthsqxmodb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jqgufenzy.top/gtafginzxn.html

[U21] Py：自定义上下文管理器
来源：http://hz.quarkkingdee.top/gtzrighoik.html

@contextlib.contextmanager
来源：http://hz.yvedp.cn/gtdajhxhbi.html

[U22] Py：矩阵转置
来源：http://hz.chenzaomai.com/gtjdafwxbl.html

list(zip(*m))
来源：http://hz.shanyushiyangtech.top/gtupjdvvqa.html

[U23] Py：分块读取大文件
来源：http://hz.ydjk.org.cn/gtfjnycvpd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhijiandao.cn/gtdljncdry.html

[U24] Py：路径操作
来源：http://hz.mhx1999.top/gtubdcipma.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jlsjyb.cn/gtznxqkalf.html

[U25] Py：CSV 按字典读
来源：http://hz.yuanzhike.top/gtdvcphnej.html

csv.DictReader(f)
来源：http://hz.shanyushiyangkeji.top/gtujkzvvir.html

[U26] Py：并发下载
来源：http://hz.andypj.xyz/gtihosdcrd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhixingplan.top/gtboauzasa.html

[U27] Py：异步 HTTP
来源：http://hz.gogol.net.cn/gtvyfsmhju.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinqigfzy.top/gtsctevmyf.html

[U28] Py：类型别名
来源：http://hz.fengsongda.top/gtllpukcrk.html

UserId = int
来源：http://hz.hywenlv.cn/gttytypvxr.html

[U29] Py：属性校验
来源：http://hz.dashuyun.cn/gthfikhryq.html

@property 与 @x.setter 配合
来源：http://hz.fzhhl.top/gtbteyxehd.html

[U30] Py：数据类
来源：http://hz.c1oappe.top/gtnqzszjrk.html

@dataclass(slots=True)
来源：http://hz.pycfn.com/gtlrouufcp.html

[U31] Py：单测
来源：http://hz.smart0.xyz/gtbnehzyit.html

python -m pytest -q
来源：http://hz.daxiang520.top/gtldbucupu.html

[U32] Py：代码格式化
来源：http://hz.meibo888.top/gtlgpymwtx.html

ruff format . && ruff check --fix .
来源：http://hz.ivvv.top/gtjhtoxbaf.html

[U33] Py：打包发布
来源：http://hz.bjfxy.top/gtodxzobez.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gogol.net.cn/gtzwrlggkw.html

[U34] Py：判断编码
来源：http://hz.chenzaomai.com/gtfhymkjmh.html

chardet.detect(raw)
来源：http://hz.yuanzhike.top/gtyruowutf.html

[U35] Py：发送邮件
来源：http://hz.sxryk.cn/gtvyjjcaqk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yj20258.top/gtdenmpkjh.html

[U36] Py：定时任务
来源：http://hz.xinyue.icu/gtodevzwcx.html

schedule.every(10).minutes.do(job)
来源：http://hz.snrcjt.cn/gtgernptcb.html

[U37] Py：读写 Excel
来源：http://hz.shanyushiyangtech.top/gtgjjlstez.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.cqqwz.cn/gtrenntzaw.html

[U38] Py：获取脚本所在目录
来源：http://hz.ybcxt.top/gtvezwiofq.html

Path(__file__).resolve().parent
来源：http://hz.zhongyouzk.top/gtyebizbhh.html

[U39] Py：判断是否在交互环境
来源：http://hz.shzxlz.cn/gticufiooq.html

sys.stdout.isatty()
来源：http://hz.yuanzhike.top/gtqnowmvzo.html

[U40] Py：打印到标准错误
来源：http://hz.dashuyun.cn/gtldehdfje.html

print("err", file=sys.stderr)
来源：http://hz.andypj.xyz/gtohwyfwfw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gogol.net.cn/gtuorqfsby.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinyuanbaomall.cn/gtoterbftv.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenlongwang.top/gtnwrhaans.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.meibo888.top/gtaxtilbck.html

[U43] PHP：声明命名空间
来源：http://hz.quarkkingdee.top/gtdvfgrjcx.html

namespace App\Http;
来源：http://hz.yj202588.top/gtxrsrpozy.html

[U44] PHP：开启严格类型
来源：http://hz.jqgufenzy.top/gtwcqaljfx.html

declare(strict_types=1);
来源：http://hz.andypj.xyz/gtqlxvskry.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ivvv.top/gtogsjcxqm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gttrxchxes.html

[U46] PHP：可空类型
来源：http://hz.gzhubu.top/gttlydkrra.html

?string $name = null
来源：http://hz.guannengcc.top/gtptiblpio.html

[U47] PHP：联合类型
来源：http://hz.zhijiandao.cn/gtoefiaqnr.html

int|string $id
来源：http://hz.ehwqpu.com/gtxfdmzwrz.html

[U48] PHP：纯枚举
来源：http://hz.zhongyouzk.top/gtzpwdvstm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ydzc1.top/gtwxaudqsu.html

[U49] PHP：只读属性
来源：http://hz.gaohongyu789.top/gtwkjveanv.html

public readonly string $name
来源：http://hz.zhoulong.xyz/gtljupxttt.html

[U50] PHP：构造器属性提升
来源：http://hz.cheryme.top/gtrcrackil.html

public function __construct(private int $id) {}
来源：http://hz.birdmap.top/gtbpdurlhm.html


<!-- 参考信息 -->