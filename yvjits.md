代发 wailian999

#ifndef X_H
来源：http://hz.gaohongyu789.top/gtizwcchdc.html

#define X_H
来源：http://hz.dianchejie.cn/gtzkkxqbyu.html

#endif
来源：http://hz.svipenyu.cn/gtgwsfulyx.html

[S31] C++：Hello World
来源：http://hz.52xcode.cn/gtkillyvfs.html

#include <iostream>
来源：http://hz.nanxuanxn.top/gtttrwiugj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sxryk.cn/gtwwobvaxf.html

[S32] C++：字符串
来源：http://hz.smart0.xyz/gtbaegieni.html

std::string s = "hi";  s += "!";
来源：http://hz.hnxiangtu.top/gtdztfuylp.html

[S33] C++：vector 增删
来源：http://hz.hysaishi.cn/gtoxovxate.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj202588.top/gtrawntozy.html

[S34] C++：遍历 vector
来源：http://hz.xylfe.cn/gtokhxmitw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yanxiufei.cn/gtmpmvibam.html

[S35] C++：map
来源：http://hz.nanxinkj.top/gtiuzlywgm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtiqztuwrl.html

[S36] C++：unordered_map
来源：http://hz.fengsongda.top/gtyaityqmj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hywenlv.cn/gtmxhposks.html

[S37] C++：set
来源：http://hz.zhaomingkeji.xyz/gtobkrwxsx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ywan-chungtsiang.top/gteazreldf.html

[S38] C++：排序
来源：http://hz.jinqigfzy.top/gtynrgmvmy.html

std::sort(v.begin(), v.end());
来源：http://hz.jinyuanbaomall.cn/gtpwlnmljg.html

[S39] C++：自定义比较器排序
来源：http://hz.yongpay.top/gtbrggvbem.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhaomingkeji.xyz/gtqnniipmf.html

[S40] C++：查找元素
来源：http://hz.cdnleiting.top/gtuuqnojbi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.daxiang520.top/gtxdyxzgtn.html

[S41] C++：类与构造函数
来源：http://hz.zhaomingkeji.xyz/gtwzqmkemd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.dashuyun.cn/gtvkupgjeh.html

[S42] C++：继承与虚函数
来源：http://hz.hfpthk.cn/gthorlftvh.html

class B : public Base { public: void f() override {} };
来源：http://hz.guowangkeji.top/gtfteiissj.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gtfwdfxwbe.html

auto p = std::make_unique<int>(5);
来源：http://hz.ehwqpu.com/gtdnlevter.html

[S44] C++：引用传参
来源：http://hz.jinghuilouyu.cn/gtbbeehato.html

void inc(int &x) { ++x; }
来源：http://hz.sxryk.cn/gtsgkriqvh.html

[S45] C++：lambda
来源：http://hz.ywan-chungtsiang.top/gtrocjmvfu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yj20258888.top/gtmzqebqvu.html

[S46] C++：函数模板
来源：http://hz.cqqwz.cn/gthnswqxie.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.dianchejie.cn/gtdnsztiwv.html

[S47] C++：结构化绑定遍历
来源：http://hz.9152youxi.cn/gtlmzfssgh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangshuangyany.cn/gtcefjvtos.html

[S48] C++：逐行读文件
来源：http://hz.xziqi.cn/gtfpdukaqk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shuidangran.top/gtryqrdbhd.html

while (std::getline(in, line)) { }
来源：http://hz.hammf.cn/gtznvlofly.html

[S49] C++：写文件
来源：http://hz.jinqigfzy.top/gtismdjkau.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sufxvd.cn/gtcvgutbah.html

[S50] C++：格式化数字
来源：http://hz.bjfxy.top/gttbzgdnoz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nanxuanxn.top/gtwykhdzhh.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtecsxpvhq.html

static_cast<double>(a) / b
来源：http://hz.zdqjudy.top/gtapfuhbpu.html

[S52] C++：const 与 noexcept
来源：http://hz.xuetiantiany.cn/gtthsgevjw.html

int size() const noexcept { return n_; }
来源：http://hz.birdmap.top/gtqdranpmm.html

[S53] C++：移动语义
来源：http://hz.guannengcc.top/gtywwoxfhz.html

std::vector<int> w = std::move(v);
来源：http://hz.xuanzx.com/gtysowwond.html

[S54] C++：异常处理
来源：http://hz.xuetiantiany.cn/gthqrtybxj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cdnleiting.top/gtnfjvistw.html

[S55] C++：结构化绑定
来源：http://hz.pycfn.com/gtiiavrzvs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.snrcjt.cn/gtburjokkd.html

[S56] C++：optional
来源：http://hz.svipenyu.cn/gtsnqizyml.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.pengpengdd.cyou/gtcmwugqyw.html

[S57] C++：编译期常量
来源：http://hz.xylfe.cn/gtprtlyoii.html

constexpr int N = 10;
来源：http://hz.gotoacloud.top/gtjucuglir.html

[S58] C++：命名空间
来源：http://hz.birdmap.top/gtiicqwhrc.html

namespace ns { int f() { return 1; } }
来源：http://hz.chenlongwang.top/gtuleqpelh.html

[S59] C++：静态断言
来源：http://hz.meibo888.top/gtvosvzrmb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cucudq.cn/gtcmrpflnt.html

[S60] C++：遍历并删除元素
来源：http://hz.sysykeji.top/gtbkfqxsdk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nanxinkj.top/gttelmeioo.html

================================================================================
来源：http://hz.nanxuanxn.top/gtmdzvryqd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydzc1.top/gtwyvkzgml.html

================================================================================
来源：http://hz.yj202588.top/gtfmwrwljg.html

[T01] Kotlin：Hello World
来源：http://hz.jinyuanbaomall.cn/gtxfpiwjmn.html

println("Hello")
来源：http://hz.nanxuanxn.top/gtapflqydt.html

[T02] Kotlin：变量
来源：http://hz.bjfxy.top/gtcagwgpid.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinghuilouyu.cn/gtvsogecsx.html

[T03] Kotlin：字符串模板
来源：http://hz.sufxvd.cn/gtdybulyvf.html

"值: $b"
来源：http://hz.0kj1m.cn/gtygueulsc.html

[T04] Kotlin：空安全
来源：http://hz.jyoumei.cn/gtmqbnptmu.html

val n: String? = null;  n?.length
来源：http://hz.cucudq.cn/gtvyczyznh.html

[T05] Kotlin：when 表达式
来源：http://hz.mhx1999.top/gtparfutzd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jiagoushi.top/gtzxrtzlog.html

[T06] Kotlin：集合映射
来源：http://hz.shzxlz.cn/gtplsddjze.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenlongwang.top/gtqwmxjezk.html

[T07] Kotlin：集合过滤
来源：http://hz.fengsongda.top/gtlcxdhted.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.havefunace.top/gtcgvwfsjd.html

[T08] Kotlin：数据类
来源：http://hz.yueranfly.top/gtyqsvrebp.html

data class User(val name: String, val age: Int)
来源：http://hz.haohaochexian.top/gtxlsoyobz.html

[T09] Kotlin：扩展函数
来源：http://hz.bjfxy.top/gtaeltbjaw.html

fun String.exclaim() = this + "!"
来源：http://hz.c1oappe.top/gtjgdysxye.html

[T10] Kotlin：默认参数
来源：http://hz.cashguo.top/gtouhrsipc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgfzy.top/gtkkvfwuqx.html

[T11] Kotlin：协程
来源：http://hz.hfpthk.cn/gtxttzttfp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.meibo888.top/gtfyeyfofh.html

[T12] Kotlin：解构声明
来源：http://hz.havefunace.top/gtoytfhaqf.html

val (a, b) = Pair(1, 2)
来源：http://hz.havefunace.top/gttcgcpvrp.html

[T13] Kotlin：只读 Map
来源：http://hz.quarkkingdee.top/gtzcdvvqtd.html

val m = mapOf("a" to 1)
来源：http://hz.xingfuxueyuan.xyz/gterevkghu.html

[T14] Kotlin：循环
来源：http://hz.fengsongda.top/gtdfwwtemc.html

for (i in 1..10) println(i)
来源：http://hz.cheryme.top/gtnmkwzgxw.html

[T15] Kotlin：接口
来源：http://hz.ehwqpu.com/gtbhjkwaqh.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258.top/gtdtsyyyna.html

[T16] Swift：Hello World
来源：http://hz.tian-w.cn/gtbheelvua.html

print("Hello")
来源：http://hz.zhaomingkeji.xyz/gtfhgydkyj.html

[T17] Swift：变量与常量
来源：http://hz.tanke756.top/gtslxcjivt.html

var a = 1;  let b = 2
来源：http://hz.yj20258888.top/gthtdsjimo.html

[T18] Swift：字符串插值
来源：http://hz.kuanghao11.cn/gtolmeynqz.html

"值: \(b)"
来源：http://hz.ydjk.org.cn/gtqayptula.html

[T19] Swift：可选绑定
来源：http://hz.0kj1m.cn/gtleywfwma.html

if let n = opt { print(n) }
来源：http://hz.zdqjudy.top/gtdpbqzkst.html

[T20] Swift：数组操作
来源：http://hz.shanyushiyangtech.top/gthtqdvulf.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigufen.top/gtkwakliic.html

[T21] Swift：遍历
来源：http://hz.zdqjudy.top/gtmmmjmfwo.html

for x in a { print(x) }
来源：http://hz.redwolf501.top/gtdhevpmoh.html

[T22] Swift：字典
来源：http://hz.zhongyouzk.top/gtenzbfuag.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tian-w.cn/gtbgnudsfe.html

[T23] Swift：函数
来源：http://hz.jinqigufen.top/gtjqolqdoj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cheryme.top/gtkuuoibcv.html

[T24] Swift：闭包
来源：http://hz.jiagoushi.top/gtxbanlvdm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shzxlz.cn/gtyxsbojww.html

[T25] Swift：结构体
来源：http://hz.wangshuangyany.cn/gtdpzvjhew.html

struct P { var x: Int }
来源：http://hz.jinqigufen.top/gtzdusmszu.html

[T26] Swift：类与重写
来源：http://hz.xylfe.cn/gtmtagjjjy.html

class A: Base { override func f() {} }
来源：http://hz.zycfv.cn/gtonnvjcsj.html

[T27] Swift：错误处理
来源：http://hz.fengsongda.top/gtayjnhmdd.html

do { try f() } catch { print(error) }
来源：http://hz.meibo888.top/gtgcmfbayv.html

[T28] Swift：枚举
来源：http://hz.smart0.xyz/gtpfirrxqc.html

enum Color { case red, green }
来源：http://hz.316326.xyz/gtpztpeodu.html

[T29] Swift：guard 提前返回
来源：http://hz.c1oappe.top/gtxnowvrki.html

guard let x = opt else { return }
来源：http://hz.zhaomingkeji.xyz/gtkazwydtc.html

[T30] Swift：协议
来源：http://hz.guannengcc.top/gtapuczkxx.html

protocol Shape { func area() -> Double }
来源：http://hz.redwolf501.top/gtozbvnret.html

[T31] Lua：Hello World
来源：http://hz.sxryk.cn/gtqbuxxbjm.html

print("Hello")
来源：http://hz.jinqigfzy.top/gtqnznadhi.html

[T32] Lua：局部变量
来源：http://hz.wangdashe.top/gtlxxrzlzy.html

local a = 1
来源：http://hz.tianlin.xyz/gtstgeklpb.html

[T33] Lua：表（数组）
来源：http://hz.yanxiufei.cn/gticwagits.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.smart0.xyz/gtjdvubpdk.html

[T34] Lua：遍历表
来源：http://hz.zhixingplan.top/gtwxpxippr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.snrcjt.cn/gtivflxpcc.html

[T35] Lua：字典表
来源：http://hz.jinghuilouyu.cn/gtmmhnojol.html

local d = { a = 1 };  d.b = 2
来源：http://hz.chenzaomai.com/gtsropfuep.html

[T36] Lua：函数
来源：http://hz.wangdashe.top/gtvffkncam.html

function add(a, b) return a + b end
来源：http://hz.zhaomingkeji.xyz/gtjewiztgt.html

[T37] Lua：字符串拼接
来源：http://hz.nanxuanxn.top/gtricvaqst.html

"a" .. "b"
来源：http://hz.quarkkingdee.top/gtfpjpsmlc.html

[T38] Lua：条件
来源：http://hz.wangdashe.top/gtviskmhde.html

if x > 0 then print("正") end
来源：http://hz.gzhubu.top/gtmtvtiepe.html

[T39] Lua：模式匹配
来源：http://hz.pycfn.com/gtsxewpkxb.html

string.find(s, "%d+")
来源：http://hz.vqdsnc.cn/gtggxzlyio.html

[T40] Lua：元表
来源：http://hz.guowangkeji.top/gtbrxdsiqp.html

setmetatable({}, { __index = base })
来源：http://hz.jqgufenzy.top/gtpsqofzhk.html

[T41] Perl：Hello World
来源：http://hz.hfpthk.cn/gtiubsgqpp.html

print "Hello\n";
来源：http://hz.jlsjyb.cn/gtrlupdvpv.html

[T42] Perl：变量类型
来源：http://hz.jinqigufen.top/gtwqhbmgxt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.9152youxi.cn/gtylutmjhl.html

[T43] Perl：字符串插值
来源：http://hz.guowangkeji.top/gthkwuudwg.html

"值: $a"
来源：http://hz.chenzaomai.com/gtswyppowu.html

[T44] Perl：条件
来源：http://hz.dianchejie.cn/gthiygkpzx.html

if ($a > 0) { print "正"; }
来源：http://hz.cheryme.top/gtsglagbiy.html

[T45] Perl：数组遍历
来源：http://hz.vqdsnc.cn/gtuyudlnmw.html

for my $x (@arr) { print $x; }
来源：http://hz.cqqwz.cn/gtqoutwevp.html

[T46] Perl：哈希操作
来源：http://hz.yj20258.top/gtqjvvbvpa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hywenlv.cn/gtssxwbzlm.html

[T47] Perl：正则捕获
来源：http://hz.xuanzx.com/gtvpwidycs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.redwolf501.top/gtxqjwykkb.html

[T48] Perl：正则替换
来源：http://hz.gaohongyu789.top/gtnzumqpwp.html

$s =~ s/old/new/g;
来源：http://hz.tianlin.xyz/gtmupqltzr.html

[T49] Perl：函数
来源：http://hz.guannengcc.top/gtaztftzsr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhixingplan.top/gtgtezlqqm.html

[T50] Perl：逐行读文件
来源：http://hz.fengsongda.top/gtsdjxyzwl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.nanxinkj.top/gtireczpri.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.sxryk.cn/gtqvymhkzb.html

[T51] Scala：Hello World
来源：http://hz.xinyue.icu/gtkycioqwl.html

println("Hello")
来源：http://hz.zhongyouzk.top/gtxcfbsauw.html

[T52] Scala：变量
来源：http://hz.xinyue.icu/gtqhtamcjf.html

val a = 1;  var b = 2
来源：http://hz.hammf.cn/gtawicpnro.html

[T53] Scala：字符串插值
来源：http://hz.daxiang520.top/gtuxyggjbi.html

s"值: $b"
来源：http://hz.birdmap.top/gtemylwhxb.html

[T54] Scala：集合映射
来源：http://hz.sweek.top/gtilltnyqn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.wangshuangyany.cn/gtzskzbpsl.html

[T55] Scala：集合过滤
来源：http://hz.yj20258888.top/gtpzjldqnq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ppjwa.cn/gtwnrhyyme.html

[T56] Scala：样例类
来源：http://hz.0kj1m.cn/gtcxargxrk.html

case class User(name: String, age: Int)
来源：http://hz.yonumen.top/gtkchlrvxz.html

[T57] Scala：模式匹配
来源：http://hz.shuidangran.top/gtggvqhuek.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xuanzx.com/gtcgeypfpo.html

[T58] Scala：函数定义
来源：http://hz.yuanzhike.top/gtbbuvkqio.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cashguo.top/gtyiqzqyow.html

[T59] Scala：循环
来源：http://hz.zhijiandao.cn/gtejzklhpk.html

for (i <- 1 to 10) println(i)
来源：http://hz.xylfe.cn/gthkwgdwkr.html

[T60] Scala：折叠
来源：http://hz.tianlin.xyz/gtnrxmjixh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gotoacloud.top/gtruzhqktb.html

================================================================================
来源：http://hz.haohaochexian.top/gtynkaivlt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.dianchejie.cn/gtzmoffwfa.html

================================================================================
来源：http://hz.yonumen.top/gtjbeyuyys.html

[U01] Py：创建虚拟环境
来源：http://hz.sysykeji.top/gtpbnnilog.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.andypj.xyz/gttmbeyyww.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhongyouzk.top/gtlbjrggdr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xinyue.icu/gtnxtnrjwg.html

[U03] Py：加载 .env 配置
来源：http://hz.c1oappe.top/gtaykcyhah.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jinqigufen.top/gtzxzackod.html

[U04] Py：变量调试打印
来源：http://hz.jinghuilouyu.cn/gtdnydvomo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sxryk.cn/gtoflknqdr.html

[U05] Py：列表去重且保序
来源：http://hz.jiagoushi.top/gtagheoizy.html

list(dict.fromkeys(arr))
来源：http://hz.zdqjudy.top/gtagqbucbx.html

[U06] Py：合并两个字典
来源：http://hz.hongshengwenyu.top/gtbyslmyeg.html

{**a, **b}
来源：http://hz.zhoulong.xyz/gtmdromzdf.html

[U07] Py：反转字典键值
来源：http://hz.jianghu66.top/gtjzscppvt.html

{v: k for k, v in d.items()}
来源：http://hz.316326.xyz/gtrlsrbtpr.html

[U08] Py：展平二维列表
来源：http://hz.cdnleiting.top/gttdwrbros.html

[y for x in nested for y in x]
来源：http://hz.hongshengwenyu.top/gtplutnghq.html

[U09] Py：字典取最大值的键
来源：http://hz.kuanghao11.cn/gtronxucew.html

max(d, key=d.get)
来源：http://hz.sysykeji.top/gtjuizsiky.html

[U10] Py：按值排序字典
来源：http://hz.gaohongyu789.top/gtkbueatmv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.guowangkeji.top/gthvjkufjy.html

[U11] Py：生成器表达式
来源：http://hz.yj202588.top/gtehguhddd.html

(x * 2 for x in arr)
来源：http://hz.ywan-chungtsiang.top/gtkudeplib.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ydzc1.top/gtenavgzus.html

Counter(arr).most_common(3)
来源：http://hz.vqdsnc.cn/gtvughbwrp.html

[U13] Py：固定长度队列
来源：http://hz.zdqjudy.top/gtlxntodzf.html

deque(maxlen=10)
来源：http://hz.mhx1999.top/gtrjgulzkv.html

[U14] Py：分组收集到列表
来源：http://hz.c1oappe.top/gtamxqobxt.html

defaultdict(list)
来源：http://hz.cqqwz.cn/gtbrpmtqur.html

[U15] Py：高精度计时
来源：http://hz.andypj.xyz/gtrcftgsdf.html

t = time.perf_counter()
来源：http://hz.feifeiyinyue.top/gtjdwvxmen.html

[U16] Py：命令行参数解析
来源：http://hz.meibo888.top/gtfuapjtdi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gzhubu.top/gtcvgoeaur.html

[U17] Py：初始化日志
来源：http://hz.jinyuanbaomall.cn/gtkjmihsmr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.meibo888.top/gtoxbgauek.html

[U18] Py：预编译正则
来源：http://hz.wangdashe.top/gttwxbsupw.html

pat = re.compile(r"\d+")
来源：http://hz.chenlongwang.top/gtydinwpwm.html

[U19] Py：正则替换带回调
来源：http://hz.pycfn.com/gtfmywhqwf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhixingplan.top/gtxwqjxaat.html

[U20] Py：缓存函数结果
来源：http://hz.yanxiufei.cn/gtrettvzry.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shangyingyoupin.top/gtbyjexrgt.html

[U21] Py：自定义上下文管理器
来源：http://hz.birdmap.top/gtpgxgschv.html

@contextlib.contextmanager
来源：http://hz.jyoumei.cn/gtztncsznj.html

[U22] Py：矩阵转置
来源：http://hz.zhixingplan.top/gthllvqoex.html

list(zip(*m))
来源：http://hz.guowangkeji.top/gtdjfiyolh.html

[U23] Py：分块读取大文件
来源：http://hz.xingfuxueyuan.xyz/gturogiats.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.andypj.xyz/gtjjozlhgu.html

[U24] Py：路径操作
来源：http://hz.wangdashe.top/gtokgpopzg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ybcxt.top/gttzrpuqur.html

[U25] Py：CSV 按字典读
来源：http://hz.cdnleiting.top/gtyhgvcjcx.html

csv.DictReader(f)
来源：http://hz.zdqjudy.top/gtihvbyzvv.html

[U26] Py：并发下载
来源：http://hz.sysykeji.top/gtttxltcop.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhengqikj.top/gtcayatyie.html

[U27] Py：异步 HTTP
来源：http://hz.hammf.cn/gtrwmlqica.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.bjfxy.top/gtywyvbtkk.html

[U28] Py：类型别名
来源：http://hz.chenlongwang.top/gtmnyegcrm.html

UserId = int
来源：http://hz.dashuyun.cn/gtfspimhrm.html

[U29] Py：属性校验
来源：http://hz.shangyingyoupin.top/gtyiteaewr.html

@property 与 @x.setter 配合
来源：http://hz.jqgufenzy.top/gtnlqxsoul.html

[U30] Py：数据类
来源：http://hz.yj20258888.top/gteeuiojua.html

@dataclass(slots=True)
来源：http://hz.tian-w.cn/gtpktzkbdp.html

[U31] Py：单测
来源：http://hz.cucudq.cn/gtcuisozon.html

python -m pytest -q
来源：http://hz.svipenyu.cn/gtjwsbbqrr.html

[U32] Py：代码格式化
来源：http://hz.sysykeji.top/gtggkfuahq.html

ruff format . && ruff check --fix .
来源：http://hz.bjfxy.top/gtppakwmdm.html

[U33] Py：打包发布
来源：http://hz.cashguo.top/gtgtjtaekj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zdqjudy.top/gtpfdegkcx.html

[U34] Py：判断编码
来源：http://hz.iojbl.cn/gtedobsqiz.html

chardet.detect(raw)
来源：http://hz.tian-w.cn/gtjceggkad.html

[U35] Py：发送邮件
来源：http://hz.zhaomingkeji.xyz/gtnciateiw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yonumen.top/gtjbuijwma.html

[U36] Py：定时任务
来源：http://hz.yanxiufei.cn/gthgpynwsz.html

schedule.every(10).minutes.do(job)
来源：http://hz.shuidangran.top/gtpvyzwctd.html

[U37] Py：读写 Excel
来源：http://hz.kuanghao11.cn/gtkvsjvevj.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yanxiufei.cn/gtvkqnaxkn.html

[U38] Py：获取脚本所在目录
来源：http://hz.ehwqpu.com/gtjusskvvj.html

Path(__file__).resolve().parent
来源：http://hz.kuanghao11.cn/gtddsiejgk.html

[U39] Py：判断是否在交互环境
来源：http://hz.9152youxi.cn/gtowrxttys.html

sys.stdout.isatty()
来源：http://hz.yj20258888.top/gtvwvhzris.html

[U40] Py：打印到标准错误
来源：http://hz.vqdsnc.cn/gtdfbfqmxp.html

print("err", file=sys.stderr)
来源：http://hz.hysaishi.cn/gtdpskmwee.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sysykeji.top/gtvziyhyoo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinqigfzy.top/gtozanvrkw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hongshengwenyu.top/gtvbzigdmw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hywenlv.cn/gtnunokhfs.html

[U43] PHP：声明命名空间
来源：http://hz.dianchejie.cn/gtwgmlgwzm.html

namespace App\Http;
来源：http://hz.gzhubu.top/gtxtnrxkse.html

[U44] PHP：开启严格类型
来源：http://hz.chenzaomai.com/gtsbkxxokx.html

declare(strict_types=1);
来源：http://hz.52xcode.cn/gtrsuxvcuc.html

[U45] PHP：类型声明与返回类型
来源：http://hz.nanxinkj.top/gtdxfbxklq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gtuoatuvej.html

[U46] PHP：可空类型
来源：http://hz.gaohongyu789.top/gtcoylqppd.html

?string $name = null
来源：http://hz.ivvv.top/gtjtrsquov.html

[U47] PHP：联合类型
来源：http://hz.jiagoushi.top/gtbtpnvgqw.html

int|string $id
来源：http://hz.daria6918.cn/gtwzamygec.html

[U48] PHP：纯枚举
来源：http://hz.guannengcc.top/gtfptelaql.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yongpay.top/gtzizynwxm.html

[U49] PHP：只读属性
来源：http://hz.smart0.xyz/gtlhxpoaqe.html

public readonly string $name
来源：http://hz.gogol.net.cn/gtcuojogkn.html

[U50] PHP：构造器属性提升
来源：http://hz.nanxuanxn.top/gtnvyssdmt.html

public function __construct(private int $id) {}
来源：http://hz.zhiwuduotai.top/gtydmcqobg.html

[U51] PHP：数组解构
来源：http://hz.nanxinkj.top/gtyvhzgrhm.html

[$a, $b] = $arr;
来源：http://hz.c1oappe.top/gtylurvpmh.html

[U52] PHP：箭头函数
来源：http://hz.birdmap.top/gtuhfawznf.html

$double = fn($x) => $x * 2;
来源：http://hz.xuetiantiany.cn/gtkeyiiifu.html

[U53] PHP：空合并运算符
来源：http://hz.zhoulong.xyz/gtfmkmkvns.html

$v = $a ?? $b ?? "default";
来源：http://hz.cheryme.top/gtjoepmxyn.html

[U54] PHP：空安全调用
来源：http://hz.zhengqikj.top/gtwmctouax.html

$obj?->method()
来源：http://hz.9152youxi.cn/gthgalatpo.html


<!-- 参考信息 -->