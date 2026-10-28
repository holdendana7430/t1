代发 wailian999

memset(a, 0, sizeof a);
来源：http://hz.jinqigfzy.top/gtbjxmoype.html

[S27] C：定义常量
来源：http://hz.yvedp.cn/gtzggdewno.html

const double PI = 3.14159;
来源：http://hz.xuanzx.com/gthnlizumn.html

[S28] C：静态变量
来源：http://hz.ydjk.org.cn/gtfyjdncau.html

static int counter = 0;
来源：http://hz.zycfv.cn/gtpvtafgoc.html

[S29] C：变参函数
来源：http://hz.cashguo.top/gtpitbvgip.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenjidiqi.icu/gtrbmyumbn.html

[S30] C：头文件保护
来源：http://hz.tianlin.xyz/gtzxzzoiet.html

#ifndef X_H
来源：http://hz.hnqzz.top/gtzghfuvae.html

#define X_H
来源：http://hz.haohaochexian.top/gtlnonjtii.html

#endif
来源：http://hz.hysaishi.cn/gtujefhkpw.html

[S31] C++：Hello World
来源：http://hz.shanyushiyangkeji.top/gtvealwwmw.html

#include <iostream>
来源：http://hz.guannengcc.top/gtvcwduyrj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aizwys.cn/gtyxanhhvj.html

[S32] C++：字符串
来源：http://hz.yanxiufei.cn/gtwfavzvzf.html

std::string s = "hi";  s += "!";
来源：http://hz.0kj1m.cn/gtoyzbgpkv.html

[S33] C++：vector 增删
来源：http://hz.sxryk.cn/gttcshjyjy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.snrcjt.cn/gtuqykkuhp.html

[S34] C++：遍历 vector
来源：http://hz.chenjidiqi.icu/gterlumtdl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.guowangkeji.top/gtspvesgns.html

[S35] C++：map
来源：http://hz.chenlongwang.top/gtsgmkvwvq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gtmdtstlcl.html

[S36] C++：unordered_map
来源：http://hz.jianghu66.top/gtvktferfk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fengsongda.top/gttdsxooio.html

[S37] C++：set
来源：http://hz.fengsongda.top/gtympmkejk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.guowangkeji.top/gtssqcuqae.html

[S38] C++：排序
来源：http://hz.jianghu66.top/gtopahoady.html

std::sort(v.begin(), v.end());
来源：http://hz.havefunace.top/gtbdnmkhcu.html

[S39] C++：自定义比较器排序
来源：http://hz.cdnleiting.top/gtzeapphcp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shzxlz.cn/gtvzpxpnlf.html

[S40] C++：查找元素
来源：http://hz.zhoulong.xyz/gtswsudgec.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jlsjyb.cn/gtiimkfoqv.html

[S41] C++：类与构造函数
来源：http://hz.hysaishi.cn/gtreckpxtv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cashguo.top/gtoexjdogw.html

[S42] C++：继承与虚函数
来源：http://hz.pycfn.com/gtlvusabsl.html

class B : public Base { public: void f() override {} };
来源：http://hz.shangyingyoupin.top/gtalcuskhk.html

[S43] C++：智能指针
来源：http://hz.zhaomingkeji.xyz/gtsdvfldsp.html

auto p = std::make_unique<int>(5);
来源：http://hz.cqqwz.cn/gtnofyxnrr.html

[S44] C++：引用传参
来源：http://hz.chenzaomai.com/gttdcuofij.html

void inc(int &x) { ++x; }
来源：http://hz.pycfn.com/gtvaiawssa.html

[S45] C++：lambda
来源：http://hz.c1oappe.top/gthooqjbyc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxinkj.top/gtsbmfyktc.html

[S46] C++：函数模板
来源：http://hz.hysaishi.cn/gtvkuqodxj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.dashuyun.cn/gtzmyoodot.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhiwuduotai.top/gteeuggbxr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gthmgswgzn.html

[S48] C++：逐行读文件
来源：http://hz.snrcjt.cn/gtbqiuroid.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yanxiufei.cn/gttwtuxdyt.html

while (std::getline(in, line)) { }
来源：http://hz.jianghu66.top/gtbufykxbv.html

[S49] C++：写文件
来源：http://hz.cheryme.top/gtjybjbjqe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cashguo.top/gtepmzrfcu.html

[S50] C++：格式化数字
来源：http://hz.yonumen.top/gtubtlzqeb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuetiantiany.cn/gtrlcxgova.html

[S51] C++：显式类型转换
来源：http://hz.tian-w.cn/gtmehuqolq.html

static_cast<double>(a) / b
来源：http://hz.xinyue.icu/gttltnvaih.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxuanxn.top/gtsleasrgd.html

int size() const noexcept { return n_; }
来源：http://hz.fengsongda.top/gtgnoklmpl.html

[S53] C++：移动语义
来源：http://hz.kuanghao11.cn/gtdobymane.html

std::vector<int> w = std::move(v);
来源：http://hz.jinghuilouyu.cn/gtvarmfntx.html

[S54] C++：异常处理
来源：http://hz.hongshengwenyu.top/gtjndhnzbi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.smart0.xyz/gtwqnnrvcc.html

[S55] C++：结构化绑定
来源：http://hz.gaohongyu789.top/gttkcrdhij.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.fengsongda.top/gtpusxnswl.html

[S56] C++：optional
来源：http://hz.zhaomingkeji.xyz/gthopdrkyc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhaomingkeji.xyz/gtucxbatyd.html

[S57] C++：编译期常量
来源：http://hz.jiagoushi.top/gtrcjhuozz.html

constexpr int N = 10;
来源：http://hz.316326.xyz/gtiivkdncc.html

[S58] C++：命名空间
来源：http://hz.9152youxi.cn/gttydhvbfu.html

namespace ns { int f() { return 1; } }
来源：http://hz.316326.xyz/gtqnqcmifw.html

[S59] C++：静态断言
来源：http://hz.gaohongyu789.top/gtyepzgbku.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yuxming.cn/gtbzfeccgf.html

[S60] C++：遍历并删除元素
来源：http://hz.yj20258888.top/gtkjhyhyec.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hywenlv.cn/gtdeuwudzz.html

================================================================================
来源：http://hz.andypj.xyz/gtphxmrkpr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cqqwz.cn/gtmfpltjsg.html

================================================================================
来源：http://hz.daxiang520.top/gtnspaqcrf.html

[T01] Kotlin：Hello World
来源：http://hz.svipenyu.cn/gtjoswmeet.html

println("Hello")
来源：http://hz.xuanzx.com/gtnatwosdl.html

[T02] Kotlin：变量
来源：http://hz.ybcxt.top/gtiowhsvll.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.bjfxy.top/gtkomonmpt.html

[T03] Kotlin：字符串模板
来源：http://hz.0kj1m.cn/gtrywhjfsm.html

"值: $b"
来源：http://hz.shangyingyoupin.top/gtmbcgylsz.html

[T04] Kotlin：空安全
来源：http://hz.zycfv.cn/gtuenxxymm.html

val n: String? = null;  n?.length
来源：http://hz.jinyuanbaomall.cn/gtzldbsdus.html

[T05] Kotlin：when 表达式
来源：http://hz.meibo888.top/gtbasrykcs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangdashe.top/gtmcmcbiog.html

[T06] Kotlin：集合映射
来源：http://hz.jinghuilouyu.cn/gtyhzaflfk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.feifeiyinyue.top/gteinzinhe.html

[T07] Kotlin：集合过滤
来源：http://hz.c1oappe.top/gtckxdxjvs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sweek.top/gtrtrgdnfe.html

[T08] Kotlin：数据类
来源：http://hz.snrcjt.cn/gtfflivccu.html

data class User(val name: String, val age: Int)
来源：http://hz.sxryk.cn/gthcrvjfjc.html

[T09] Kotlin：扩展函数
来源：http://hz.xuetiantiany.cn/gthprawpud.html

fun String.exclaim() = this + "!"
来源：http://hz.shanyushiyangkeji.top/gtkdwvmros.html

[T10] Kotlin：默认参数
来源：http://hz.xuanzx.com/gtzkfzdlxx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.quarkkingdee.top/gtjowzwfdp.html

[T11] Kotlin：协程
来源：http://hz.wangdashe.top/gtjxgyqpyz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.svipenyu.cn/gtpbzesdno.html

[T12] Kotlin：解构声明
来源：http://hz.zhaomingkeji.xyz/gtxgtwwyph.html

val (a, b) = Pair(1, 2)
来源：http://hz.jianghu66.top/gtipmqdrig.html

[T13] Kotlin：只读 Map
来源：http://hz.aizwys.cn/gthrudfenu.html

val m = mapOf("a" to 1)
来源：http://hz.zhixingplan.top/gtlixnitll.html

[T14] Kotlin：循环
来源：http://hz.xuanzx.com/gtidtimynn.html

for (i in 1..10) println(i)
来源：http://hz.mhx1999.top/gtiakfrckm.html

[T15] Kotlin：接口
来源：http://hz.ydjk.org.cn/gtumqczlkl.html

interface Shape { fun area(): Double }
来源：http://hz.guowangkeji.top/gtdbahlont.html

[T16] Swift：Hello World
来源：http://hz.jianghu66.top/gtdxjsduvl.html

print("Hello")
来源：http://hz.sysykeji.top/gtystjxgrf.html

[T17] Swift：变量与常量
来源：http://hz.xinyue.icu/gtqtkgbdqr.html

var a = 1;  let b = 2
来源：http://hz.dianchejie.cn/gtdpmiqdks.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangtech.top/gtcxhatqyi.html

"值: \(b)"
来源：http://hz.sufxvd.cn/gtwmepnbtd.html

[T19] Swift：可选绑定
来源：http://hz.chenzaomai.com/gtbwkeived.html

if let n = opt { print(n) }
来源：http://hz.cdnleiting.top/gtftrwwwei.html

[T20] Swift：数组操作
来源：http://hz.jlsjyb.cn/gtuaspbkfm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hywenlv.cn/gtegzhamvp.html

[T21] Swift：遍历
来源：http://hz.zhongyouzk.top/gtpdpueqpi.html

for x in a { print(x) }
来源：http://hz.zhixingplan.top/gthshodjem.html

[T22] Swift：字典
来源：http://hz.meibo888.top/gtfhzplqzh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.dianchejie.cn/gtxlwakkgt.html

[T23] Swift：函数
来源：http://hz.tianlin.xyz/gtbqtfuzwy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.wangshuangyany.cn/gtcjtxlajt.html

[T24] Swift：闭包
来源：http://hz.zhongyouzk.top/gtatpzwwdf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xinyue.icu/gtlalfyflh.html

[T25] Swift：结构体
来源：http://hz.yangfankeji.com/gtjdcnards.html

struct P { var x: Int }
来源：http://hz.daria6918.cn/gtqrjvlagd.html

[T26] Swift：类与重写
来源：http://hz.yuanzhike.top/gtwivzfsly.html

class A: Base { override func f() {} }
来源：http://hz.tianlin.xyz/gtmrooxftf.html

[T27] Swift：错误处理
来源：http://hz.ppjwa.cn/gtweqwjwat.html

do { try f() } catch { print(error) }
来源：http://hz.jinghuilouyu.cn/gtldilzevb.html

[T28] Swift：枚举
来源：http://hz.tianlin.xyz/gtgjktdwvb.html

enum Color { case red, green }
来源：http://hz.jinqigfzy.top/gtoexxeiob.html

[T29] Swift：guard 提前返回
来源：http://hz.cdnleiting.top/gtsrodcznr.html

guard let x = opt else { return }
来源：http://hz.yuxming.cn/gttvgsxlxr.html

[T30] Swift：协议
来源：http://hz.svipenyu.cn/gtdymrtiix.html

protocol Shape { func area() -> Double }
来源：http://hz.jqgufenzy.top/gtkclsmbjm.html

[T31] Lua：Hello World
来源：http://hz.zhijiandao.cn/gttuaureox.html

print("Hello")
来源：http://hz.yueranfly.top/gtdcektkfe.html

[T32] Lua：局部变量
来源：http://hz.jqgfzy.top/gtgddzpgit.html

local a = 1
来源：http://hz.ydzc1.top/gtgfrldtth.html

[T33] Lua：表（数组）
来源：http://hz.0kj1m.cn/gtzndldryc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hywenlv.cn/gtkztslwsm.html

[T34] Lua：遍历表
来源：http://hz.sysykeji.top/gtupdjzxlk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hammf.cn/gtvinbyvjo.html

[T35] Lua：字典表
来源：http://hz.zhiwuduotai.top/gtypplqihr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.fzhhl.top/gtqinxevci.html

[T36] Lua：函数
来源：http://hz.cashguo.top/gtdvjhaxxp.html

function add(a, b) return a + b end
来源：http://hz.chenlongwang.top/gtlrchdltd.html

[T37] Lua：字符串拼接
来源：http://hz.wangdashe.top/gttlgfuyuc.html

"a" .. "b"
来源：http://hz.xingfuxueyuan.xyz/gtmdwqgppj.html

[T38] Lua：条件
来源：http://hz.iojbl.cn/gthjbwliib.html

if x > 0 then print("正") end
来源：http://hz.jianghu66.top/gthrffmcnt.html

[T39] Lua：模式匹配
来源：http://hz.jiagoushi.top/gtwdwcgroa.html

string.find(s, "%d+")
来源：http://hz.9152youxi.cn/gtpjpewffj.html

[T40] Lua：元表
来源：http://hz.sysykeji.top/gtnjfkijyt.html

setmetatable({}, { __index = base })
来源：http://hz.daxiang520.top/gtuekywswg.html

[T41] Perl：Hello World
来源：http://hz.tanke756.top/gtmxqcxvvb.html

print "Hello\n";
来源：http://hz.shanyushiyangtech.top/gtyvqcyjod.html

[T42] Perl：变量类型
来源：http://hz.yangfankeji.com/gtwcpfascs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yueranfly.top/gtxxdllqfu.html

[T43] Perl：字符串插值
来源：http://hz.aibaodan.cn/gtjsqxkvum.html

"值: $a"
来源：http://hz.yj20258.top/gtzvqyhjpw.html

[T44] Perl：条件
来源：http://hz.shangyingyoupin.top/gtoiimpxig.html

if ($a > 0) { print "正"; }
来源：http://hz.gzhubu.top/gtowwbrgig.html

[T45] Perl：数组遍历
来源：http://hz.zhaomingkeji.xyz/gtivtsvvxy.html

for my $x (@arr) { print $x; }
来源：http://hz.yanxiufei.cn/gtvpnvblms.html

[T46] Perl：哈希操作
来源：http://hz.yueranfly.top/gtqytpiesl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hongshengwenyu.top/gtrrelddpd.html

[T47] Perl：正则捕获
来源：http://hz.yj202588.top/gtbledajhs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhixingplan.top/gtthuqdxym.html

[T48] Perl：正则替换
来源：http://hz.zycfv.cn/gtjwzprooh.html

$s =~ s/old/new/g;
来源：http://hz.yangfankeji.com/gtdpluybvl.html

[T49] Perl：函数
来源：http://hz.hongshengwenyu.top/gtflfivpre.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.dashuyun.cn/gtzguivsjr.html

[T50] Perl：逐行读文件
来源：http://hz.kuanghao11.cn/gthegifimq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zycfv.cn/gtuqxgdfco.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hongshengwenyu.top/gttixxvsbl.html

[T51] Scala：Hello World
来源：http://hz.zycfv.cn/gtpiamvkbc.html

println("Hello")
来源：http://hz.hfpthk.cn/gthvzpmvxk.html

[T52] Scala：变量
来源：http://hz.cqqwz.cn/gtiwqezxex.html

val a = 1;  var b = 2
来源：http://hz.xuetiantiany.cn/gtzhzdswhc.html

[T53] Scala：字符串插值
来源：http://hz.chenzaomai.com/gtmljhyclc.html

s"值: $b"
来源：http://hz.zhoulong.xyz/gtksfydjyv.html

[T54] Scala：集合映射
来源：http://hz.zhijiandao.cn/gtqbixpbvn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.pycfn.com/gtwqxnopge.html

[T55] Scala：集合过滤
来源：http://hz.zycfv.cn/gtgpinonne.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hywenlv.cn/gtdkokxkcx.html

[T56] Scala：样例类
来源：http://hz.tianlin.xyz/gtnghwtxpa.html

case class User(name: String, age: Int)
来源：http://hz.zhijiandao.cn/gtzvoivhrp.html

[T57] Scala：模式匹配
来源：http://hz.smart0.xyz/gtrmwpgefd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jiagoushi.top/gtaqtvzjiq.html

[T58] Scala：函数定义
来源：http://hz.tianlin.xyz/gtesffarnv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.mhx1999.top/gtzbruchsx.html

[T59] Scala：循环
来源：http://hz.pycfn.com/gtnbhikoon.html

for (i <- 1 to 10) println(i)
来源：http://hz.daxiang520.top/gteesemcii.html

[T60] Scala：折叠
来源：http://hz.bjfxy.top/gtqsqsuvpl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gzhubu.top/gtnppsgyvw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtbivwbjet.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sxryk.cn/gtkhlzquoo.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtezvkpdmm.html

[U01] Py：创建虚拟环境
来源：http://hz.nwbrower.top/gtowtgcpuu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.feifeiyinyue.top/gtiapgexjw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cqqwz.cn/gtuzdapgsa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gotoacloud.top/gtdoaahzia.html

[U03] Py：加载 .env 配置
来源：http://hz.sufxvd.cn/gtayrwhuxp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.quarkkingdee.top/gtxoruoovp.html

[U04] Py：变量调试打印
来源：http://hz.dianchejie.cn/gtujddqawr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinyuanbaomall.cn/gtufiwtsqm.html

[U05] Py：列表去重且保序
来源：http://hz.xziqi.cn/gtvpjmnhnl.html

list(dict.fromkeys(arr))
来源：http://hz.xuanzx.com/gtjqctohrz.html

[U06] Py：合并两个字典
来源：http://hz.smart0.xyz/gtkdiqeldg.html

{**a, **b}
来源：http://hz.hnqzz.top/gtahlgamgu.html

[U07] Py：反转字典键值
来源：http://hz.shangyingyoupin.top/gtdriacfjw.html

{v: k for k, v in d.items()}
来源：http://hz.zhoulong.xyz/gtiksobvmq.html

[U08] Py：展平二维列表
来源：http://hz.iojbl.cn/gtpdudhoul.html

[y for x in nested for y in x]
来源：http://hz.nanxinkj.top/gtpgighrtr.html

[U09] Py：字典取最大值的键
来源：http://hz.haohaochexian.top/gtotoctcrc.html

max(d, key=d.get)
来源：http://hz.sysykeji.top/gtpcvkiamq.html

[U10] Py：按值排序字典
来源：http://hz.cucudq.cn/gtbbluvuif.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ivvv.top/gtbgpldvmw.html

[U11] Py：生成器表达式
来源：http://hz.yvedp.cn/gtvuvslexl.html

(x * 2 for x in arr)
来源：http://hz.tianlin.xyz/gtejnlppve.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.meibo888.top/gtnyielfnp.html

Counter(arr).most_common(3)
来源：http://hz.ivvv.top/gtxpsrflwv.html

[U13] Py：固定长度队列
来源：http://hz.hysaishi.cn/gthhanehmp.html

deque(maxlen=10)
来源：http://hz.yongpay.top/gtkwmcszrt.html

[U14] Py：分组收集到列表
来源：http://hz.wangshuangyany.cn/gtstqkufor.html

defaultdict(list)
来源：http://hz.birdmap.top/gtdvstnlfm.html

[U15] Py：高精度计时
来源：http://hz.jianghu66.top/gtkxryywyz.html

t = time.perf_counter()
来源：http://hz.havefunace.top/gthwkuxxsk.html

[U16] Py：命令行参数解析
来源：http://hz.jqgfzy.top/gtwcpiktal.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cucudq.cn/gtvxujgwcw.html

[U17] Py：初始化日志
来源：http://hz.nanxuanxn.top/gtodidtnlj.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xuetiantiany.cn/gtvqsrhzhv.html

[U18] Py：预编译正则
来源：http://hz.0kj1m.cn/gteskadnyk.html

pat = re.compile(r"\d+")
来源：http://hz.guannengcc.top/gtshylwvuq.html

[U19] Py：正则替换带回调
来源：http://hz.xuetiantiany.cn/gtpllmxhrj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.feifeiyinyue.top/gtqabtoudf.html

[U20] Py：缓存函数结果
来源：http://hz.gogol.net.cn/gthynmvmon.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hnxiangtu.top/gtexfdciak.html

[U21] Py：自定义上下文管理器
来源：http://hz.xingfuxueyuan.xyz/gtpoacdfgu.html

@contextlib.contextmanager
来源：http://hz.cqqwz.cn/gtpsrwxgnv.html

[U22] Py：矩阵转置
来源：http://hz.shangyingyoupin.top/gtilwyrhxp.html

list(zip(*m))
来源：http://hz.andypj.xyz/gtpoclphhz.html

[U23] Py：分块读取大文件
来源：http://hz.hnxiangtu.top/gtirqwqfgz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ydzc1.top/gthsktkybn.html

[U24] Py：路径操作
来源：http://hz.meibo888.top/gtawqnhggr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.smart0.xyz/gtdzhnszai.html

[U25] Py：CSV 按字典读
来源：http://hz.jlsjyb.cn/gtmfneaegt.html

csv.DictReader(f)
来源：http://hz.zhiwuduotai.top/gtegiqvhvv.html

[U26] Py：并发下载
来源：http://hz.jinghuilouyu.cn/gtqmmfsmes.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shangyingyoupin.top/gtpuftlota.html

[U27] Py：异步 HTTP
来源：http://hz.wangdashe.top/gtnadevbbu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.iojbl.cn/gtijaqqjzd.html

[U28] Py：类型别名
来源：http://hz.shzxlz.cn/gtfsbwhudx.html

UserId = int
来源：http://hz.shanyushiyangtech.top/gtszvjpqwq.html

[U29] Py：属性校验
来源：http://hz.ybcxt.top/gtvmrawuic.html

@property 与 @x.setter 配合
来源：http://hz.yj20258888.top/gtybjlpcdq.html

[U30] Py：数据类
来源：http://hz.vqdsnc.cn/gtptarixor.html

@dataclass(slots=True)
来源：http://hz.birdmap.top/gthtdecrte.html

[U31] Py：单测
来源：http://hz.jinyuanbaomall.cn/gtcdkzszww.html

python -m pytest -q
来源：http://hz.shzxlz.cn/gtiazevlbn.html

[U32] Py：代码格式化
来源：http://hz.hfpthk.cn/gtqrlfjezk.html

ruff format . && ruff check --fix .
来源：http://hz.jyoumei.cn/gtbkbfddpt.html

[U33] Py：打包发布
来源：http://hz.jinqigufen.top/gtcgknkbic.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.dianchejie.cn/gthshddmud.html

[U34] Py：判断编码
来源：http://hz.dianchejie.cn/gtzftuadsx.html

chardet.detect(raw)
来源：http://hz.yuxming.cn/gtwserdotl.html

[U35] Py：发送邮件
来源：http://hz.smart0.xyz/gtplhqhwou.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.fzhhl.top/gtdrwoyoha.html

[U36] Py：定时任务
来源：http://hz.yanxiufei.cn/gtwwcqhjrm.html

schedule.every(10).minutes.do(job)
来源：http://hz.redwolf501.top/gtdpitvsvw.html

[U37] Py：读写 Excel
来源：http://hz.jinqigufen.top/gtgwnxqkgb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shuidangran.top/gtelzutleb.html

[U38] Py：获取脚本所在目录
来源：http://hz.fengsongda.top/gtwzijovrk.html

Path(__file__).resolve().parent
来源：http://hz.zhengqikj.top/gtqkiwobqq.html

[U39] Py：判断是否在交互环境
来源：http://hz.yonumen.top/gttzqxrxoy.html

sys.stdout.isatty()
来源：http://hz.sufxvd.cn/gtjphalvwo.html

[U40] Py：打印到标准错误
来源：http://hz.52xcode.cn/gtqklvqhha.html

print("err", file=sys.stderr)
来源：http://hz.zhongyouzk.top/gtjlomrhlv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinqigufen.top/gtkbynhhlv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.9152youxi.cn/gtxwtppxca.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.snrcjt.cn/gtieiznqlv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.smart0.xyz/gtqyggcqor.html

[U43] PHP：声明命名空间
来源：http://hz.jqgufenzy.top/gtdaaxkexd.html

namespace App\Http;
来源：http://hz.hammf.cn/gtnhgptyas.html

[U44] PHP：开启严格类型
来源：http://hz.snrcjt.cn/gtkjnetnpk.html

declare(strict_types=1);
来源：http://hz.jinyuanbaomall.cn/gtfupusows.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yonumen.top/gtpohuqjxk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jianghu66.top/gtddwoafcf.html

[U46] PHP：可空类型
来源：http://hz.jiagoushi.top/gtylulsjdc.html

?string $name = null
来源：http://hz.ywan-chungtsiang.top/gtpbdesyle.html

[U47] PHP：联合类型
来源：http://hz.gogol.net.cn/gtnexekfpx.html

int|string $id
来源：http://hz.cucudq.cn/gtyesmwabe.html

[U48] PHP：纯枚举
来源：http://hz.yj20258888.top/gthscoonqd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.svipenyu.cn/gtaveiiyfa.html

[U49] PHP：只读属性
来源：http://hz.gotoacloud.top/gtmvqegnlg.html

public readonly string $name
来源：http://hz.ppjwa.cn/gtmffgddil.html

[U50] PHP：构造器属性提升
来源：http://hz.cqqwz.cn/gtaljrddpl.html

public function __construct(private int $id) {}
来源：http://hz.hysaishi.cn/gttkdjmfnf.html


<!-- 参考信息 -->