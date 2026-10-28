代发 wailian999

memset(a, 0, sizeof a);
来源：http://hz.wangshuangyany.cn/gtsbpztnxd.html

[S27] C：定义常量
来源：http://hz.dashuyun.cn/gtpisrydzp.html

const double PI = 3.14159;
来源：http://hz.pycfn.com/gtuygdpzmm.html

[S28] C：静态变量
来源：http://hz.ybcxt.top/gtjdxjkygy.html

static int counter = 0;
来源：http://hz.dashuyun.cn/gtabogkntu.html

[S29] C：变参函数
来源：http://hz.haohaochexian.top/gtucxhvqgo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.redwolf501.top/gtgrhahicx.html

[S30] C：头文件保护
来源：http://hz.jqgufenzy.top/gtmtjplmoo.html

#ifndef X_H
来源：http://hz.daria6918.cn/gtburadstt.html

#define X_H
来源：http://hz.zhiwuduotai.top/gtmjxycouo.html

#endif
来源：http://hz.hysaishi.cn/gtqlqzkhwn.html

[S31] C++：Hello World
来源：http://hz.birdmap.top/gtckdghqyd.html

#include <iostream>
来源：http://hz.gotoacloud.top/gtgslamvph.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.0kj1m.cn/gtlmllmysj.html

[S32] C++：字符串
来源：http://hz.guowangkeji.top/gtospmjbss.html

std::string s = "hi";  s += "!";
来源：http://hz.feifeiyinyue.top/gtapzchnzv.html

[S33] C++：vector 增删
来源：http://hz.chenjidiqi.icu/gtnvcoprol.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.chenlongwang.top/gtqrchnlku.html

[S34] C++：遍历 vector
来源：http://hz.cashguo.top/gthfgpegik.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj202588.top/gtcfcprqik.html

[S35] C++：map
来源：http://hz.yangfankeji.com/gtoenzklmd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtqdmejmwd.html

[S36] C++：unordered_map
来源：http://hz.feifeiyinyue.top/gtqrxqlvrv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gtbgmefdcm.html

[S37] C++：set
来源：http://hz.xziqi.cn/gtplfqjvjf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydjk.org.cn/gtuzyhzkbt.html

[S38] C++：排序
来源：http://hz.ehwqpu.com/gtumgvwlra.html

std::sort(v.begin(), v.end());
来源：http://hz.aibaodan.cn/gtcrepowhs.html

[S39] C++：自定义比较器排序
来源：http://hz.yvedp.cn/gtbpijofxd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydzc1.top/gtplvpzpkt.html

[S40] C++：查找元素
来源：http://hz.hammf.cn/gtadzfamnu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.feifeiyinyue.top/gtkuwqwzfj.html

[S41] C++：类与构造函数
来源：http://hz.sweek.top/gtpdymvohv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhaomingkeji.xyz/gttbdnutvn.html

[S42] C++：继承与虚函数
来源：http://hz.yj20258.top/gtgmcihgox.html

class B : public Base { public: void f() override {} };
来源：http://hz.ywan-chungtsiang.top/gtxncgmiaf.html

[S43] C++：智能指针
来源：http://hz.xuanzx.com/gtfqmyrnix.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj20258.top/gtmjhhjzxl.html

[S44] C++：引用传参
来源：http://hz.sxryk.cn/gtberfflfn.html

void inc(int &x) { ++x; }
来源：http://hz.zhoulong.xyz/gthewdguni.html

[S45] C++：lambda
来源：http://hz.316326.xyz/gtowefnzip.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hfpthk.cn/gtzjpoqdtj.html

[S46] C++：函数模板
来源：http://hz.feifeiyinyue.top/gttxyboube.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gotoacloud.top/gtmamwotvn.html

[S47] C++：结构化绑定遍历
来源：http://hz.guowangkeji.top/gtaxkdolin.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yangfankeji.com/gtpqhzrpdo.html

[S48] C++：逐行读文件
来源：http://hz.chenjidiqi.icu/gthztjcbhh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhiwuduotai.top/gtecejpphj.html

while (std::getline(in, line)) { }
来源：http://hz.316326.xyz/gtsekalgdb.html

[S49] C++：写文件
来源：http://hz.jinyuanbaomall.cn/gtowwuzccw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xuanzx.com/gtifuwsgye.html

[S50] C++：格式化数字
来源：http://hz.shangyingyoupin.top/gtpaxochbo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gzhubu.top/gtnsxkerxj.html

[S51] C++：显式类型转换
来源：http://hz.jqgfzy.top/gteojepcxm.html

static_cast<double>(a) / b
来源：http://hz.yuxming.cn/gtjcbvwidx.html

[S52] C++：const 与 noexcept
来源：http://hz.fengsongda.top/gtgitrnudy.html

int size() const noexcept { return n_; }
来源：http://hz.ydjk.org.cn/gtrbuablio.html

[S53] C++：移动语义
来源：http://hz.aizwys.cn/gtwmrimnnz.html

std::vector<int> w = std::move(v);
来源：http://hz.yonumen.top/gtqshwahgt.html

[S54] C++：异常处理
来源：http://hz.gotoacloud.top/gtthirjyke.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shuidangran.top/gthguzyxwy.html

[S55] C++：结构化绑定
来源：http://hz.hnxiangtu.top/gtdlknidwv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shanyushiyangkeji.top/gtbitabdjl.html

[S56] C++：optional
来源：http://hz.ppjwa.cn/gtjflmwzuo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xylfe.cn/gtzcicgwlp.html

[S57] C++：编译期常量
来源：http://hz.chenlongwang.top/gtejhxctro.html

constexpr int N = 10;
来源：http://hz.redwolf501.top/gtpgxxpohd.html

[S58] C++：命名空间
来源：http://hz.yuanzhike.top/gtrbistkpr.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgfzy.top/gtultltflo.html

[S59] C++：静态断言
来源：http://hz.ppjwa.cn/gtqgusflod.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.haohaochexian.top/gtsqgkwfcj.html

[S60] C++：遍历并删除元素
来源：http://hz.yongpay.top/gtwlzkryal.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yonumen.top/gtnquxvtuk.html

================================================================================
来源：http://hz.chenzaomai.com/gtjmzjzfwc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj202588.top/gtdvjeltca.html

================================================================================
来源：http://hz.fengsongda.top/gtoaogsyge.html

[T01] Kotlin：Hello World
来源：http://hz.shangyingyoupin.top/gtovnnyqau.html

println("Hello")
来源：http://hz.svipenyu.cn/gtlrfqkbui.html

[T02] Kotlin：变量
来源：http://hz.bjfxy.top/gtepwmzwya.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shuidangran.top/gtccewwrxc.html

[T03] Kotlin：字符串模板
来源：http://hz.ppjwa.cn/gtmfesevqz.html

"值: $b"
来源：http://hz.chenzaomai.com/gtqvcrplxz.html

[T04] Kotlin：空安全
来源：http://hz.zhoulong.xyz/gthjtgekel.html

val n: String? = null;  n?.length
来源：http://hz.pycfn.com/gtmkemlrnq.html

[T05] Kotlin：when 表达式
来源：http://hz.dashuyun.cn/gtnuykjusy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.redwolf501.top/gtisqqeeza.html

[T06] Kotlin：集合映射
来源：http://hz.zhaomingkeji.xyz/gtejhoyajn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.316326.xyz/gtnnimsjjv.html

[T07] Kotlin：集合过滤
来源：http://hz.nanxinkj.top/gtpogohjjj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xuetiantiany.cn/gtiskuggta.html

[T08] Kotlin：数据类
来源：http://hz.xuetiantiany.cn/gtygxgfvmg.html

data class User(val name: String, val age: Int)
来源：http://hz.0kj1m.cn/gtyhoziwmp.html

[T09] Kotlin：扩展函数
来源：http://hz.shangyingyoupin.top/gtiojslqmp.html

fun String.exclaim() = this + "!"
来源：http://hz.cdnleiting.top/gtchqsolzj.html

[T10] Kotlin：默认参数
来源：http://hz.hongshengwenyu.top/gtndpspohn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ppjwa.cn/gtpwlbynqg.html

[T11] Kotlin：协程
来源：http://hz.redwolf501.top/gtnbstcvci.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.nanxinkj.top/gtmelzonlt.html

[T12] Kotlin：解构声明
来源：http://hz.yuanzhike.top/gtkrxzowtc.html

val (a, b) = Pair(1, 2)
来源：http://hz.mhx1999.top/gtbhflgchs.html

[T13] Kotlin：只读 Map
来源：http://hz.hammf.cn/gtqzqlojdi.html

val m = mapOf("a" to 1)
来源：http://hz.jinghuilouyu.cn/gtrqvegoab.html

[T14] Kotlin：循环
来源：http://hz.pengpengdd.cyou/gtsdhrmwcm.html

for (i in 1..10) println(i)
来源：http://hz.jinghuilouyu.cn/gtedvdpxkq.html

[T15] Kotlin：接口
来源：http://hz.chenlongwang.top/gtdpjyjonl.html

interface Shape { fun area(): Double }
来源：http://hz.52xcode.cn/gtoagirflz.html

[T16] Swift：Hello World
来源：http://hz.zhijiandao.cn/gtwgkhrozf.html

print("Hello")
来源：http://hz.cdnleiting.top/gtilolzclh.html

[T17] Swift：变量与常量
来源：http://hz.redwolf501.top/gtlcjmjncs.html

var a = 1;  let b = 2
来源：http://hz.xuetiantiany.cn/gtdccawqtp.html

[T18] Swift：字符串插值
来源：http://hz.dashuyun.cn/gtzoyjslia.html

"值: \(b)"
来源：http://hz.zhijiandao.cn/gtawgccpwb.html

[T19] Swift：可选绑定
来源：http://hz.sweek.top/gtkbvlmxao.html

if let n = opt { print(n) }
来源：http://hz.yj20258888.top/gtfkljtaac.html

[T20] Swift：数组操作
来源：http://hz.wangdashe.top/gtttcrijgs.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.9152youxi.cn/gtxlkuymmd.html

[T21] Swift：遍历
来源：http://hz.yongpay.top/gthxbjwpmg.html

for x in a { print(x) }
来源：http://hz.yj20258.top/gtoyhnyirg.html

[T22] Swift：字典
来源：http://hz.xziqi.cn/gtpustgtls.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ydjk.org.cn/gtbbofjrny.html

[T23] Swift：函数
来源：http://hz.shanyushiyangkeji.top/gtypcrrtmj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.redwolf501.top/gtqilbgdhi.html

[T24] Swift：闭包
来源：http://hz.hywenlv.cn/gtxxbqghru.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.316326.xyz/gtxwmmqsyx.html

[T25] Swift：结构体
来源：http://hz.shangyingyoupin.top/gtvrrbciiy.html

struct P { var x: Int }
来源：http://hz.hfpthk.cn/gtpqtpnwbr.html

[T26] Swift：类与重写
来源：http://hz.shanyushiyangtech.top/gttdnsscmb.html

class A: Base { override func f() {} }
来源：http://hz.yj20258888.top/gtjdlvsbed.html

[T27] Swift：错误处理
来源：http://hz.chenjidiqi.icu/gtlaeuzqwb.html

do { try f() } catch { print(error) }
来源：http://hz.ivvv.top/gtflyoqjvc.html

[T28] Swift：枚举
来源：http://hz.c1oappe.top/gtynodhovb.html

enum Color { case red, green }
来源：http://hz.pycfn.com/gtjpwzgbam.html

[T29] Swift：guard 提前返回
来源：http://hz.smart0.xyz/gtxmicetsz.html

guard let x = opt else { return }
来源：http://hz.iojbl.cn/gtawbfbzdi.html

[T30] Swift：协议
来源：http://hz.wangshuangyany.cn/gtvkjjfzhi.html

protocol Shape { func area() -> Double }
来源：http://hz.mhx1999.top/gtaoakibqq.html

[T31] Lua：Hello World
来源：http://hz.zycfv.cn/gtmhnllymu.html

print("Hello")
来源：http://hz.zycfv.cn/gtwzojqcvo.html

[T32] Lua：局部变量
来源：http://hz.hongshengwenyu.top/gtgzeejfbr.html

local a = 1
来源：http://hz.yvedp.cn/gtnstpmvgv.html

[T33] Lua：表（数组）
来源：http://hz.daria6918.cn/gtixwibvmp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.52xcode.cn/gtmrhrrwvf.html

[T34] Lua：遍历表
来源：http://hz.fzhhl.top/gtymscyjso.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.smart0.xyz/gtfcfagwbq.html

[T35] Lua：字典表
来源：http://hz.xziqi.cn/gtecpsjfto.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xziqi.cn/gtupeoghji.html

[T36] Lua：函数
来源：http://hz.nanxinkj.top/gtafhgehqo.html

function add(a, b) return a + b end
来源：http://hz.shanyushiyangtech.top/gtsqewambw.html

[T37] Lua：字符串拼接
来源：http://hz.jinghuilouyu.cn/gtyfkqfzgl.html

"a" .. "b"
来源：http://hz.zhaomingkeji.xyz/gtonvsllvj.html

[T38] Lua：条件
来源：http://hz.shanyushiyangkeji.top/gtewkyggop.html

if x > 0 then print("正") end
来源：http://hz.kuanghao11.cn/gtyhowlqfy.html

[T39] Lua：模式匹配
来源：http://hz.ywan-chungtsiang.top/gtzmsciwfn.html

string.find(s, "%d+")
来源：http://hz.cashguo.top/gtzilzgrqv.html

[T40] Lua：元表
来源：http://hz.xinyue.icu/gtmlcjgpye.html

setmetatable({}, { __index = base })
来源：http://hz.bjfxy.top/gtnubrghni.html

[T41] Perl：Hello World
来源：http://hz.cucudq.cn/gtrsjuyrlw.html

print "Hello\n";
来源：http://hz.haohaochexian.top/gtnahqjnyz.html

[T42] Perl：变量类型
来源：http://hz.jinyuanbaomall.cn/gtskfvqokk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sweek.top/gtwjrxasba.html

[T43] Perl：字符串插值
来源：http://hz.yongpay.top/gtrdpizioq.html

"值: $a"
来源：http://hz.andypj.xyz/gtksspgwel.html

[T44] Perl：条件
来源：http://hz.hammf.cn/gtwxcijebh.html

if ($a > 0) { print "正"; }
来源：http://hz.nanxuanxn.top/gtnoitwtxq.html

[T45] Perl：数组遍历
来源：http://hz.jiagoushi.top/gtmomgwfyk.html

for my $x (@arr) { print $x; }
来源：http://hz.shanyushiyangkeji.top/gttxgmvjdf.html

[T46] Perl：哈希操作
来源：http://hz.ivvv.top/gticyvkmfb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.havefunace.top/gtwikthypx.html

[T47] Perl：正则捕获
来源：http://hz.ywan-chungtsiang.top/gttnkvujqz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ybcxt.top/gtufgmiszn.html

[T48] Perl：正则替换
来源：http://hz.wangshuangyany.cn/gtxcuchcql.html

$s =~ s/old/new/g;
来源：http://hz.snrcjt.cn/gtotpdvodz.html

[T49] Perl：函数
来源：http://hz.haohaochexian.top/gtvdecfnll.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.quarkkingdee.top/gtdvhxdijo.html

[T50] Perl：逐行读文件
来源：http://hz.dashuyun.cn/gtgpqhxzsn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.aizwys.cn/gtstsicqje.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.chenzaomai.com/gtwzpdtjkl.html

[T51] Scala：Hello World
来源：http://hz.aibaodan.cn/gttyzwnupw.html

println("Hello")
来源：http://hz.zhixingplan.top/gtyqtlvcdw.html

[T52] Scala：变量
来源：http://hz.hnqzz.top/gtswwfvxva.html

val a = 1;  var b = 2
来源：http://hz.nanxinkj.top/gtqdzossdk.html

[T53] Scala：字符串插值
来源：http://hz.nanxuanxn.top/gtdldhatwp.html

s"值: $b"
来源：http://hz.xuetiantiany.cn/gtpkpoefoj.html

[T54] Scala：集合映射
来源：http://hz.sxryk.cn/gtjxwnossl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jinyuanbaomall.cn/gtfiycmwxs.html

[T55] Scala：集合过滤
来源：http://hz.zhijiandao.cn/gtozaczmll.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhongyouzk.top/gtdkxheiai.html

[T56] Scala：样例类
来源：http://hz.xziqi.cn/gtlkwjntih.html

case class User(name: String, age: Int)
来源：http://hz.tanke756.top/gtcbnhdaie.html

[T57] Scala：模式匹配
来源：http://hz.cdnleiting.top/gtvtpdesid.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xinyue.icu/gtejcszzjc.html

[T58] Scala：函数定义
来源：http://hz.shuidangran.top/gtoutoerxc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jlsjyb.cn/gtjyijgzvu.html

[T59] Scala：循环
来源：http://hz.svipenyu.cn/gtdvljoxrv.html

for (i <- 1 to 10) println(i)
来源：http://hz.sweek.top/gtevfurmcf.html

[T60] Scala：折叠
来源：http://hz.nanxinkj.top/gttamiutwa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.bjfxy.top/gtthoagube.html

================================================================================
来源：http://hz.gaohongyu789.top/gtquwhonzh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.feifeiyinyue.top/gtoztqpgkp.html

================================================================================
来源：http://hz.guowangkeji.top/gtwtnnzgmk.html

[U01] Py：创建虚拟环境
来源：http://hz.ydzc1.top/gttgtgzvsm.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.meibo888.top/gthsnteshh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xingfuxueyuan.xyz/gtfuwdsioz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hfpthk.cn/gthtttqmdk.html

[U03] Py：加载 .env 配置
来源：http://hz.wangdashe.top/gtfjonbsgj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ivvv.top/gtjwbiadrh.html

[U04] Py：变量调试打印
来源：http://hz.fengsongda.top/gttqexricm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hywenlv.cn/gtsnipprab.html

[U05] Py：列表去重且保序
来源：http://hz.316326.xyz/gtnepjkeia.html

list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtxrkubpna.html

[U06] Py：合并两个字典
来源：http://hz.shanyushiyangkeji.top/gtngngwmmj.html

{**a, **b}
来源：http://hz.yj20258888.top/gtaegssioe.html

[U07] Py：反转字典键值
来源：http://hz.ehwqpu.com/gttwxjhtmx.html

{v: k for k, v in d.items()}
来源：http://hz.hnqzz.top/gtgywmjrfq.html

[U08] Py：展平二维列表
来源：http://hz.yanxiufei.cn/gtftsqraql.html

[y for x in nested for y in x]
来源：http://hz.nwbrower.top/gtxmfwitxk.html

[U09] Py：字典取最大值的键
来源：http://hz.wangdashe.top/gtwngrsskn.html

max(d, key=d.get)
来源：http://hz.yangfankeji.com/gttplhhaet.html

[U10] Py：按值排序字典
来源：http://hz.gaohongyu789.top/gtyzroicci.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cucudq.cn/gtpxphthkn.html

[U11] Py：生成器表达式
来源：http://hz.c1oappe.top/gtecptuhct.html

(x * 2 for x in arr)
来源：http://hz.xylfe.cn/gtuigkiedu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhiwuduotai.top/gtscmyswww.html

Counter(arr).most_common(3)
来源：http://hz.zhongyouzk.top/gtzuivlrnt.html

[U13] Py：固定长度队列
来源：http://hz.vqdsnc.cn/gtfmwmlwkn.html

deque(maxlen=10)
来源：http://hz.cheryme.top/gtwjofoggl.html

[U14] Py：分组收集到列表
来源：http://hz.xuetiantiany.cn/gtqvxoktqg.html

defaultdict(list)
来源：http://hz.xuetiantiany.cn/gtgpnnlpsn.html

[U15] Py：高精度计时
来源：http://hz.shanyushiyangkeji.top/gtrlexruci.html

t = time.perf_counter()
来源：http://hz.quarkkingdee.top/gtztnisdaw.html

[U16] Py：命令行参数解析
来源：http://hz.jinghuilouyu.cn/gtpskoicsk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jlsjyb.cn/gtpbidtqwz.html

[U17] Py：初始化日志
来源：http://hz.316326.xyz/gtruoaaipe.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ydzc1.top/gtfmtwvizo.html

[U18] Py：预编译正则
来源：http://hz.fzhhl.top/gtkuhlrmwf.html

pat = re.compile(r"\d+")
来源：http://hz.wangshuangyany.cn/gtjocuyqwg.html

[U19] Py：正则替换带回调
来源：http://hz.hnxiangtu.top/gtjthauiof.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hysaishi.cn/gtpmzwdjhr.html

[U20] Py：缓存函数结果
来源：http://hz.aizwys.cn/gtbthzakbn.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinghuilouyu.cn/gtqftnvtfv.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhiwuduotai.top/gtgeipyvrb.html

@contextlib.contextmanager
来源：http://hz.zhoulong.xyz/gtzaehztaj.html

[U22] Py：矩阵转置
来源：http://hz.zhoulong.xyz/gtnqayayht.html

list(zip(*m))
来源：http://hz.cdnleiting.top/gtdnjpbsrv.html

[U23] Py：分块读取大文件
来源：http://hz.ivvv.top/gtxvctfuyo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.52xcode.cn/gtjlhaunqj.html

[U24] Py：路径操作
来源：http://hz.wangshuangyany.cn/gtvoyuniwa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jiagoushi.top/gtzedmsdlq.html

[U25] Py：CSV 按字典读
来源：http://hz.nanxinkj.top/gtwxvvxied.html

csv.DictReader(f)
来源：http://hz.xingfuxueyuan.xyz/gtiyncrcdy.html

[U26] Py：并发下载
来源：http://hz.yuxming.cn/gtropuhzyf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhixingplan.top/gteanhtlng.html

[U27] Py：异步 HTTP
来源：http://hz.guowangkeji.top/gtvjmzgukn.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ehwqpu.com/gtkbidoofg.html

[U28] Py：类型别名
来源：http://hz.jinyuanbaomall.cn/gtdqzwqtrq.html

UserId = int
来源：http://hz.jinqigufen.top/gtfmeugodk.html

[U29] Py：属性校验
来源：http://hz.cdnleiting.top/gtgmwnvvzx.html

@property 与 @x.setter 配合
来源：http://hz.gogol.net.cn/gtvqfirpua.html

[U30] Py：数据类
来源：http://hz.hnqzz.top/gtxvesdeqm.html

@dataclass(slots=True)
来源：http://hz.haohaochexian.top/gtfwlkjjrn.html

[U31] Py：单测
来源：http://hz.nanxinkj.top/gtarkxuojd.html

python -m pytest -q
来源：http://hz.gzhubu.top/gtxzwuonnn.html

[U32] Py：代码格式化
来源：http://hz.jqgufenzy.top/gtjwigaasj.html

ruff format . && ruff check --fix .
来源：http://hz.yueranfly.top/gtvjkvmtyg.html

[U33] Py：打包发布
来源：http://hz.shangyingyoupin.top/gtwwgzbjsk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ybcxt.top/gtxtmagsfm.html

[U34] Py：判断编码
来源：http://hz.cucudq.cn/gtaqayfrjy.html

chardet.detect(raw)
来源：http://hz.zycfv.cn/gtskgdnqzl.html

[U35] Py：发送邮件
来源：http://hz.pengpengdd.cyou/gtcjcozchh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hysaishi.cn/gtvsnqmovb.html

[U36] Py：定时任务
来源：http://hz.pengpengdd.cyou/gtfyebaepy.html

schedule.every(10).minutes.do(job)
来源：http://hz.shuidangran.top/gtuifoqrez.html

[U37] Py：读写 Excel
来源：http://hz.tanke756.top/gtdcwmjqip.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.dashuyun.cn/gtfsnligfl.html

[U38] Py：获取脚本所在目录
来源：http://hz.316326.xyz/gtooobfzlg.html

Path(__file__).resolve().parent
来源：http://hz.cdnleiting.top/gtmbetskze.html

[U39] Py：判断是否在交互环境
来源：http://hz.0kj1m.cn/gtkwphbdzr.html

sys.stdout.isatty()
来源：http://hz.gzhubu.top/gtqwcmrncg.html

[U40] Py：打印到标准错误
来源：http://hz.jqgufenzy.top/gtfpizlhpv.html

print("err", file=sys.stderr)
来源：http://hz.chenzaomai.com/gtqjlugrhz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hnxiangtu.top/gtvindzgxs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ivvv.top/gtovqrpmop.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.guowangkeji.top/gtbicydgbv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.fengsongda.top/gtvxoczybt.html

[U43] PHP：声明命名空间
来源：http://hz.jinyuanbaomall.cn/gtvdwhmqfo.html

namespace App\Http;
来源：http://hz.xinyue.icu/gtinrtbhjn.html

[U44] PHP：开启严格类型
来源：http://hz.aibaodan.cn/gtrxoqslye.html

declare(strict_types=1);
来源：http://hz.jiagoushi.top/gtjqsyqxnj.html

[U45] PHP：类型声明与返回类型
来源：http://hz.havefunace.top/gthjwctigg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtiqeszmep.html

[U46] PHP：可空类型
来源：http://hz.yanxiufei.cn/gtupbesmrn.html

?string $name = null
来源：http://hz.yangfankeji.com/gthyolnolf.html

[U47] PHP：联合类型
来源：http://hz.yj20258888.top/gtlbhqcyry.html

int|string $id
来源：http://hz.9152youxi.cn/gtoprmmjqk.html

[U48] PHP：纯枚举
来源：http://hz.jiagoushi.top/gtdkxuvplj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.havefunace.top/gtljgtrngd.html

[U49] PHP：只读属性
来源：http://hz.hysaishi.cn/gtmfrfcgcb.html

public readonly string $name
来源：http://hz.daxiang520.top/gtqcqoszlm.html

[U50] PHP：构造器属性提升
来源：http://hz.ivvv.top/gtzejxcuks.html

public function __construct(private int $id) {}
来源：http://hz.gzhubu.top/gtryncwypw.html


<!-- 参考信息 -->