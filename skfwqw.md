代发 wailian999

#ifndef X_H
来源：http://hz.zycfv.cn/gtgryzqujy.html

#define X_H
来源：http://hz.guannengcc.top/gtoconvogj.html

#endif
来源：http://hz.aibaodan.cn/gthrfhmeyg.html

[S31] C++：Hello World
来源：http://hz.ydzc1.top/gtiiccmdbs.html

#include <iostream>
来源：http://hz.hysaishi.cn/gthpyvftik.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tanke756.top/gtygbywieo.html

[S32] C++：字符串
来源：http://hz.yuxming.cn/gtwzmgnxhz.html

std::string s = "hi";  s += "!";
来源：http://hz.xziqi.cn/gtxauqwpbt.html

[S33] C++：vector 增删
来源：http://hz.nanxuanxn.top/gtlzwqogbu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yonumen.top/gteeesftir.html

[S34] C++：遍历 vector
来源：http://hz.jinqigfzy.top/gtohmywyyd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.dashuyun.cn/gtxcjjqeha.html

[S35] C++：map
来源：http://hz.yvedp.cn/gtbigpzfch.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtwmcsxqez.html

[S36] C++：unordered_map
来源：http://hz.fzhhl.top/gtmnhgmlca.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtwixiblnl.html

[S37] C++：set
来源：http://hz.yonumen.top/gtoyyrqcbt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinqigfzy.top/gtuiqmpaai.html

[S38] C++：排序
来源：http://hz.ppjwa.cn/gtpvlovhms.html

std::sort(v.begin(), v.end());
来源：http://hz.9152youxi.cn/gtxxcxplef.html

[S39] C++：自定义比较器排序
来源：http://hz.feifeiyinyue.top/gtsextfbke.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shuidangran.top/gttqiqwygi.html

[S40] C++：查找元素
来源：http://hz.andypj.xyz/gtfeiafpkx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guowangkeji.top/gtydtradxv.html

[S41] C++：类与构造函数
来源：http://hz.aizwys.cn/gtgutuealc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xylfe.cn/gtaukgixdl.html

[S42] C++：继承与虚函数
来源：http://hz.ydjk.org.cn/gtxpuxkjly.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxuanxn.top/gtjwwemwuo.html

[S43] C++：智能指针
来源：http://hz.yongpay.top/gttunbwfot.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhaomingkeji.xyz/gtomjvbtdk.html

[S44] C++：引用传参
来源：http://hz.sxryk.cn/gterchsdfj.html

void inc(int &x) { ++x; }
来源：http://hz.52xcode.cn/gtixunxsem.html

[S45] C++：lambda
来源：http://hz.dashuyun.cn/gtlmlfblgc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aizwys.cn/gttzvfoqfy.html

[S46] C++：函数模板
来源：http://hz.yanxiufei.cn/gtvmluxbbf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aizwys.cn/gtjnypszva.html

[S47] C++：结构化绑定遍历
来源：http://hz.guowangkeji.top/gtmubfkvcw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhiwuduotai.top/gtjkpaarvq.html

[S48] C++：逐行读文件
来源：http://hz.shzxlz.cn/gtdsgofcll.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tian-w.cn/gtyyjjcifc.html

while (std::getline(in, line)) { }
来源：http://hz.nanxinkj.top/gtcafzjmtr.html

[S49] C++：写文件
来源：http://hz.shzxlz.cn/gtwdppdhac.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jlsjyb.cn/gtfajluyej.html

[S50] C++：格式化数字
来源：http://hz.chenzaomai.com/gtffwtkevz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigfzy.top/gtfrodbvbg.html

[S51] C++：显式类型转换
来源：http://hz.hnqzz.top/gtuwdkpugz.html

static_cast<double>(a) / b
来源：http://hz.nanxuanxn.top/gtuuxzpemj.html

[S52] C++：const 与 noexcept
来源：http://hz.jinqigufen.top/gtbrgjfbsl.html

int size() const noexcept { return n_; }
来源：http://hz.shanyushiyangtech.top/gtokrqmcex.html

[S53] C++：移动语义
来源：http://hz.chenlongwang.top/gtvljkerxu.html

std::vector<int> w = std::move(v);
来源：http://hz.jinghuilouyu.cn/gtnaiciepp.html

[S54] C++：异常处理
来源：http://hz.chenjidiqi.icu/gthurmrpww.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tanke756.top/gtlbljidkg.html

[S55] C++：结构化绑定
来源：http://hz.jyoumei.cn/gtzootxuyr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shangyingyoupin.top/gtzdhuoztp.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gtrmnxlmua.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cdnleiting.top/gtbkmmkfar.html

[S57] C++：编译期常量
来源：http://hz.cheryme.top/gtlmrawsdt.html

constexpr int N = 10;
来源：http://hz.tanke756.top/gtodsehhxu.html

[S58] C++：命名空间
来源：http://hz.jinyuanbaomall.cn/gtncdtfytr.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtmysatcpv.html

[S59] C++：静态断言
来源：http://hz.sysykeji.top/gtorizzpvf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.havefunace.top/gtxexbfwbw.html

[S60] C++：遍历并删除元素
来源：http://hz.tian-w.cn/gthlanhccf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj202588.top/gtvamcojsp.html

================================================================================
来源：http://hz.bjfxy.top/gtwwayycmj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hfpthk.cn/gtdpnkvhsm.html

================================================================================
来源：http://hz.vqdsnc.cn/gtybikcwnp.html

[T01] Kotlin：Hello World
来源：http://hz.guannengcc.top/gtavhdukxc.html

println("Hello")
来源：http://hz.guannengcc.top/gtwjuyouej.html

[T02] Kotlin：变量
来源：http://hz.0kj1m.cn/gtsfadpcvj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.andypj.xyz/gtvnpxlzjz.html

[T03] Kotlin：字符串模板
来源：http://hz.cheryme.top/gtowkjchqu.html

"值: $b"
来源：http://hz.zycfv.cn/gtcdyqgabb.html

[T04] Kotlin：空安全
来源：http://hz.jqgfzy.top/gtlkeywbse.html

val n: String? = null;  n?.length
来源：http://hz.gogol.net.cn/gtzyzjzwwa.html

[T05] Kotlin：when 表达式
来源：http://hz.ehwqpu.com/gtwzlesvka.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yonumen.top/gthnrvrsic.html

[T06] Kotlin：集合映射
来源：http://hz.nanxuanxn.top/gtbccdazqs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.pengpengdd.cyou/gtziasdpmq.html

[T07] Kotlin：集合过滤
来源：http://hz.52xcode.cn/gtlioqjlky.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nanxuanxn.top/gtaaixeamv.html

[T08] Kotlin：数据类
来源：http://hz.snrcjt.cn/gtqrdysvzw.html

data class User(val name: String, val age: Int)
来源：http://hz.zhiwuduotai.top/gtpnbwpusm.html

[T09] Kotlin：扩展函数
来源：http://hz.jinqigufen.top/gtrqrvlibi.html

fun String.exclaim() = this + "!"
来源：http://hz.tianlin.xyz/gtmfdzpwjr.html

[T10] Kotlin：默认参数
来源：http://hz.tianlin.xyz/gticdmopft.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aibaodan.cn/gtzqpccmru.html

[T11] Kotlin：协程
来源：http://hz.jinqigufen.top/gtnfcvonkf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yvedp.cn/gtvswzzrbj.html

[T12] Kotlin：解构声明
来源：http://hz.gogol.net.cn/gtpmocquip.html

val (a, b) = Pair(1, 2)
来源：http://hz.xinyue.icu/gtjdvnphaa.html

[T13] Kotlin：只读 Map
来源：http://hz.zycfv.cn/gtnydaqihc.html

val m = mapOf("a" to 1)
来源：http://hz.jqgufenzy.top/gthwtbdsfz.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gthychczrw.html

for (i in 1..10) println(i)
来源：http://hz.316326.xyz/gtfdajwppj.html

[T15] Kotlin：接口
来源：http://hz.yuanzhike.top/gtknzbjlkb.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gtwpvaaxaj.html

[T16] Swift：Hello World
来源：http://hz.chenlongwang.top/gtslnvirdz.html

print("Hello")
来源：http://hz.pengpengdd.cyou/gthqestsud.html

[T17] Swift：变量与常量
来源：http://hz.ydzc1.top/gtwwihhyex.html

var a = 1;  let b = 2
来源：http://hz.smart0.xyz/gtsmecqvax.html

[T18] Swift：字符串插值
来源：http://hz.zdqjudy.top/gtvuiygyaf.html

"值: \(b)"
来源：http://hz.c1oappe.top/gtsuwlkabu.html

[T19] Swift：可选绑定
来源：http://hz.ydjk.org.cn/gtxofdvykd.html

if let n = opt { print(n) }
来源：http://hz.shanyushiyangtech.top/gtkwbtycyw.html

[T20] Swift：数组操作
来源：http://hz.ehwqpu.com/gttvkyiuzl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yj202588.top/gtrgtgnvwh.html

[T21] Swift：遍历
来源：http://hz.jianghu66.top/gtdzyfwfvi.html

for x in a { print(x) }
来源：http://hz.sufxvd.cn/gtjnkiavnf.html

[T22] Swift：字典
来源：http://hz.gaohongyu789.top/gtmmedzwth.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ivvv.top/gtmybouxdp.html

[T23] Swift：函数
来源：http://hz.wangdashe.top/gtzpxpkmgd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yj202588.top/gtrgksafuz.html

[T24] Swift：闭包
来源：http://hz.fengsongda.top/gtvgmexfbj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gogol.net.cn/gtiziyanwi.html

[T25] Swift：结构体
来源：http://hz.gotoacloud.top/gtrjledvaq.html

struct P { var x: Int }
来源：http://hz.ivvv.top/gtyqpqpwuc.html

[T26] Swift：类与重写
来源：http://hz.xinyue.icu/gtwcwoiocm.html

class A: Base { override func f() {} }
来源：http://hz.meibo888.top/gtqbbanfsj.html

[T27] Swift：错误处理
来源：http://hz.zhoulong.xyz/gtdsgwylzz.html

do { try f() } catch { print(error) }
来源：http://hz.andypj.xyz/gtoipfdjln.html

[T28] Swift：枚举
来源：http://hz.cheryme.top/gtethkuwlf.html

enum Color { case red, green }
来源：http://hz.dashuyun.cn/gtgfmhagcn.html

[T29] Swift：guard 提前返回
来源：http://hz.ivvv.top/gtzlcaufus.html

guard let x = opt else { return }
来源：http://hz.nanxuanxn.top/gtosokmclc.html

[T30] Swift：协议
来源：http://hz.daxiang520.top/gtcbfepxoa.html

protocol Shape { func area() -> Double }
来源：http://hz.jinghuilouyu.cn/gtcblahpkt.html

[T31] Lua：Hello World
来源：http://hz.aibaodan.cn/gtcmwectrz.html

print("Hello")
来源：http://hz.daria6918.cn/gttdnahtfc.html

[T32] Lua：局部变量
来源：http://hz.cheryme.top/gtxjlixxsv.html

local a = 1
来源：http://hz.xylfe.cn/gtyyyxarpn.html

[T33] Lua：表（数组）
来源：http://hz.bjfxy.top/gtweaohbdy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cucudq.cn/gtbwyxieja.html

[T34] Lua：遍历表
来源：http://hz.ybcxt.top/gtrhapihco.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gzhubu.top/gtnqhfbotr.html

[T35] Lua：字典表
来源：http://hz.hfpthk.cn/gtbsxkftrn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yuanzhike.top/gtvymmlldf.html

[T36] Lua：函数
来源：http://hz.hysaishi.cn/gtsgnhajdu.html

function add(a, b) return a + b end
来源：http://hz.gogol.net.cn/gtenjwunpl.html

[T37] Lua：字符串拼接
来源：http://hz.cucudq.cn/gtvjmyytes.html

"a" .. "b"
来源：http://hz.shanyushiyangkeji.top/gtljxeijik.html

[T38] Lua：条件
来源：http://hz.xylfe.cn/gtdvhfseop.html

if x > 0 then print("正") end
来源：http://hz.fzhhl.top/gtzwjqbjlj.html

[T39] Lua：模式匹配
来源：http://hz.dashuyun.cn/gtweukfcms.html

string.find(s, "%d+")
来源：http://hz.fengsongda.top/gtpfhepypy.html

[T40] Lua：元表
来源：http://hz.yanxiufei.cn/gtfnotqojz.html

setmetatable({}, { __index = base })
来源：http://hz.ywan-chungtsiang.top/gtmedjiiob.html

[T41] Perl：Hello World
来源：http://hz.zhongyouzk.top/gtjsvxycuv.html

print "Hello\n";
来源：http://hz.jinqigfzy.top/gtkhwhmkbb.html

[T42] Perl：变量类型
来源：http://hz.yangfankeji.com/gtrjrqqwmt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhiwuduotai.top/gtybjcupvz.html

[T43] Perl：字符串插值
来源：http://hz.chenlongwang.top/gtmxgiruna.html

"值: $a"
来源：http://hz.tian-w.cn/gtgrnstdem.html

[T44] Perl：条件
来源：http://hz.sysykeji.top/gtpzzcassb.html

if ($a > 0) { print "正"; }
来源：http://hz.cqqwz.cn/gtvosvzrjz.html

[T45] Perl：数组遍历
来源：http://hz.redwolf501.top/gttvngrbtd.html

for my $x (@arr) { print $x; }
来源：http://hz.aizwys.cn/gtbsfzbozc.html

[T46] Perl：哈希操作
来源：http://hz.jlsjyb.cn/gtjncfcfls.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.daxiang520.top/gtzafktiwk.html

[T47] Perl：正则捕获
来源：http://hz.andypj.xyz/gtrdxxtyfr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cdnleiting.top/gtdgpbgirm.html

[T48] Perl：正则替换
来源：http://hz.aibaodan.cn/gtnyjfzaud.html

$s =~ s/old/new/g;
来源：http://hz.jinqigufen.top/gtmlpsdqvu.html

[T49] Perl：函数
来源：http://hz.snrcjt.cn/gtxjsjulgp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zycfv.cn/gtzifazqxw.html

[T50] Perl：逐行读文件
来源：http://hz.cdnleiting.top/gtnrufscrf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.quarkkingdee.top/gtffqfrxct.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hnxiangtu.top/gtuyyhxzex.html

[T51] Scala：Hello World
来源：http://hz.hammf.cn/gtdanlvekp.html

println("Hello")
来源：http://hz.zhoulong.xyz/gtjhienjcu.html

[T52] Scala：变量
来源：http://hz.0kj1m.cn/gtedjcnouv.html

val a = 1;  var b = 2
来源：http://hz.316326.xyz/gtmsogifba.html

[T53] Scala：字符串插值
来源：http://hz.fzhhl.top/gtiipoizcj.html

s"值: $b"
来源：http://hz.yj202588.top/gtrwzwutsd.html

[T54] Scala：集合映射
来源：http://hz.zycfv.cn/gtvruddvgw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhengqikj.top/gttyjktnfs.html

[T55] Scala：集合过滤
来源：http://hz.shanyushiyangtech.top/gtdyeawhou.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhaomingkeji.xyz/gtszhmczai.html

[T56] Scala：样例类
来源：http://hz.havefunace.top/gtdtdrseht.html

case class User(name: String, age: Int)
来源：http://hz.zhixingplan.top/gttdnmosom.html

[T57] Scala：模式匹配
来源：http://hz.xziqi.cn/gtgjkaulkl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ydzc1.top/gtaxrjiopg.html

[T58] Scala：函数定义
来源：http://hz.feifeiyinyue.top/gtkiuuzpga.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jyoumei.cn/gtbfebpqwh.html

[T59] Scala：循环
来源：http://hz.cqqwz.cn/gtihyszitx.html

for (i <- 1 to 10) println(i)
来源：http://hz.nwbrower.top/gtaldqzjeh.html

[T60] Scala：折叠
来源：http://hz.tian-w.cn/gtgsmwbpwk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sufxvd.cn/gttvyqisdb.html

================================================================================
来源：http://hz.sysykeji.top/gtcmumtqxz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.havefunace.top/gtyefnhkau.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtfcabrjbp.html

[U01] Py：创建虚拟环境
来源：http://hz.pengpengdd.cyou/gtahufqjhy.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.guowangkeji.top/gtxazedvoa.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sysykeji.top/gtzjvegdue.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.fzhhl.top/gtcecefmyx.html

[U03] Py：加载 .env 配置
来源：http://hz.aizwys.cn/gtoeeaohos.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sxryk.cn/gtyvygzqes.html

[U04] Py：变量调试打印
来源：http://hz.guowangkeji.top/gtevxhuzjw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zycfv.cn/gtoryosqar.html

[U05] Py：列表去重且保序
来源：http://hz.chenjidiqi.icu/gttuexlaed.html

list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gthhzxbmgg.html

[U06] Py：合并两个字典
来源：http://hz.daxiang520.top/gtjvvnfpps.html

{**a, **b}
来源：http://hz.yangfankeji.com/gtgdaefnin.html

[U07] Py：反转字典键值
来源：http://hz.quarkkingdee.top/gtqkfemkvp.html

{v: k for k, v in d.items()}
来源：http://hz.haohaochexian.top/gtocgrsemx.html

[U08] Py：展平二维列表
来源：http://hz.316326.xyz/gtbivxetzl.html

[y for x in nested for y in x]
来源：http://hz.hnxiangtu.top/gtjngoqcts.html

[U09] Py：字典取最大值的键
来源：http://hz.cashguo.top/gtraggenpt.html

max(d, key=d.get)
来源：http://hz.hongshengwenyu.top/gtwzmevvue.html

[U10] Py：按值排序字典
来源：http://hz.shangyingyoupin.top/gtzgbhpeku.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yanxiufei.cn/gtbtknhpvg.html

[U11] Py：生成器表达式
来源：http://hz.svipenyu.cn/gtihrcqhtt.html

(x * 2 for x in arr)
来源：http://hz.cashguo.top/gttjjoqicu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tanke756.top/gtyfavbsbv.html

Counter(arr).most_common(3)
来源：http://hz.havefunace.top/gtigppdwzi.html

[U13] Py：固定长度队列
来源：http://hz.jinqigfzy.top/gtvthmmjvq.html

deque(maxlen=10)
来源：http://hz.zhengqikj.top/gtouffdquw.html

[U14] Py：分组收集到列表
来源：http://hz.zhoulong.xyz/gtdtbwpphx.html

defaultdict(list)
来源：http://hz.guannengcc.top/gtgrdnodgq.html

[U15] Py：高精度计时
来源：http://hz.guowangkeji.top/gtibmbrkfg.html

t = time.perf_counter()
来源：http://hz.fengsongda.top/gtwohvnzxg.html

[U16] Py：命令行参数解析
来源：http://hz.zycfv.cn/gtfgdemalb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hysaishi.cn/gttcfvoqnz.html

[U17] Py：初始化日志
来源：http://hz.nanxinkj.top/gteehqvbpx.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yongpay.top/gtxoxqgxxt.html

[U18] Py：预编译正则
来源：http://hz.jinqigufen.top/gtdjencxrd.html

pat = re.compile(r"\d+")
来源：http://hz.cashguo.top/gtprdxziyl.html

[U19] Py：正则替换带回调
来源：http://hz.hywenlv.cn/gturfdscnt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.havefunace.top/gtqcjbcoxi.html

[U20] Py：缓存函数结果
来源：http://hz.xingfuxueyuan.xyz/gtcporomub.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xylfe.cn/gtzcwzhkeg.html

[U21] Py：自定义上下文管理器
来源：http://hz.chenlongwang.top/gtevygppez.html

@contextlib.contextmanager
来源：http://hz.yuanzhike.top/gtbdstbqzk.html

[U22] Py：矩阵转置
来源：http://hz.zycfv.cn/gtboflylno.html

list(zip(*m))
来源：http://hz.chenlongwang.top/gthwvcbbma.html

[U23] Py：分块读取大文件
来源：http://hz.yongpay.top/gtdswentfn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cashguo.top/gtwsgaybqq.html

[U24] Py：路径操作
来源：http://hz.jinqigufen.top/gtrkatxyyy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yj20258888.top/gtijyvdrlg.html

[U25] Py：CSV 按字典读
来源：http://hz.zhoulong.xyz/gtkjmeqboh.html

csv.DictReader(f)
来源：http://hz.chenzaomai.com/gtyfuiouvw.html

[U26] Py：并发下载
来源：http://hz.sufxvd.cn/gtjnypvogl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.bjfxy.top/gtpcexxtge.html

[U27] Py：异步 HTTP
来源：http://hz.gotoacloud.top/gtetclmbul.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sweek.top/gtfbydqdou.html

[U28] Py：类型别名
来源：http://hz.fengsongda.top/gthkjfexcy.html

UserId = int
来源：http://hz.sweek.top/gtqmrpzcpe.html

[U29] Py：属性校验
来源：http://hz.316326.xyz/gtyoekbnrw.html

@property 与 @x.setter 配合
来源：http://hz.gogol.net.cn/gtqkqjgwmm.html

[U30] Py：数据类
来源：http://hz.jlsjyb.cn/gtxwryzbiy.html

@dataclass(slots=True)
来源：http://hz.xinyue.icu/gthuznplrc.html

[U31] Py：单测
来源：http://hz.daria6918.cn/gtegbxjdfb.html

python -m pytest -q
来源：http://hz.jianghu66.top/gtaxcsstdb.html

[U32] Py：代码格式化
来源：http://hz.jinqigufen.top/gtkjnzqxru.html

ruff format . && ruff check --fix .
来源：http://hz.zhongyouzk.top/gtfbfurrpn.html

[U33] Py：打包发布
来源：http://hz.jyoumei.cn/gtcoortphv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xziqi.cn/gtooddscqb.html

[U34] Py：判断编码
来源：http://hz.yj202588.top/gtpkqjlubr.html

chardet.detect(raw)
来源：http://hz.cdnleiting.top/gtuztmnlzn.html

[U35] Py：发送邮件
来源：http://hz.jinyuanbaomall.cn/gthhfpkzde.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhongyouzk.top/gtakebvsjd.html

[U36] Py：定时任务
来源：http://hz.0kj1m.cn/gtiydvniad.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj20258888.top/gtcgqvcncb.html

[U37] Py：读写 Excel
来源：http://hz.daria6918.cn/gtwrkkwtvk.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.daria6918.cn/gtsvqejequ.html

[U38] Py：获取脚本所在目录
来源：http://hz.yj20258.top/gtkytoagos.html

Path(__file__).resolve().parent
来源：http://hz.sysykeji.top/gtxtmdylzn.html

[U39] Py：判断是否在交互环境
来源：http://hz.yangfankeji.com/gtvzxdssod.html

sys.stdout.isatty()
来源：http://hz.zhongyouzk.top/gtjwmmjnta.html

[U40] Py：打印到标准错误
来源：http://hz.xziqi.cn/gtxlbuxpev.html

print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gtsuditvlb.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zdqjudy.top/gtvwgfkkpu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinghuilouyu.cn/gtmmjqhjlp.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yonumen.top/gtwzwwzmrg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.iojbl.cn/gtwwijbhec.html

[U43] PHP：声明命名空间
来源：http://hz.zhaomingkeji.xyz/gtxaqowjsh.html

namespace App\Http;
来源：http://hz.ivvv.top/gtvktqecdm.html

[U44] PHP：开启严格类型
来源：http://hz.xuanzx.com/gtnzavxqlh.html

declare(strict_types=1);
来源：http://hz.tian-w.cn/gtkcdoiayl.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jlsjyb.cn/gtabtqycyq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtpzluwohi.html

[U46] PHP：可空类型
来源：http://hz.dianchejie.cn/gtbsvykces.html

?string $name = null
来源：http://hz.vqdsnc.cn/gtyptpjeat.html

[U47] PHP：联合类型
来源：http://hz.yj20258.top/gtpylxhojo.html

int|string $id
来源：http://hz.ivvv.top/gtzudkehyv.html

[U48] PHP：纯枚举
来源：http://hz.daria6918.cn/gtuscpqmnn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.316326.xyz/gtryverhiw.html

[U49] PHP：只读属性
来源：http://hz.hammf.cn/gtscysoezx.html

public readonly string $name
来源：http://hz.sufxvd.cn/gturqvenum.html

[U50] PHP：构造器属性提升
来源：http://hz.zdqjudy.top/gtswcrbwkw.html

public function __construct(private int $id) {}
来源：http://hz.ehwqpu.com/gtrauuwyuf.html

[U51] PHP：数组解构
来源：http://hz.shzxlz.cn/gtxxiecwcl.html

[$a, $b] = $arr;
来源：http://hz.fzhhl.top/gtpmkxaqte.html

[U52] PHP：箭头函数
来源：http://hz.jinqigufen.top/gtgktnykwv.html

$double = fn($x) => $x * 2;
来源：http://hz.jiagoushi.top/gtxqwyybxt.html

[U53] PHP：空合并运算符
来源：http://hz.chenjidiqi.icu/gtjtdsqiiz.html

$v = $a ?? $b ?? "default";
来源：http://hz.hysaishi.cn/gtiytospgw.html

[U54] PHP：空安全调用
来源：http://hz.birdmap.top/gtnaholfkf.html

$obj?->method()
来源：http://hz.fengsongda.top/gtlamlslwl.html


<!-- 参考信息 -->