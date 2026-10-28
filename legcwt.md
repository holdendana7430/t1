代发 wailian999

#ifndef X_H
来源：http://hz.yj20258888.top/gtuekymwrx.html

#define X_H
来源：http://hz.meibo888.top/gtptzbrjcy.html

#endif
来源：http://hz.jinghuilouyu.cn/gtoacxikwc.html

[S31] C++：Hello World
来源：http://hz.jqgfzy.top/gtkbphiigp.html

#include <iostream>
来源：http://hz.ywan-chungtsiang.top/gtdootrpxp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.fengsongda.top/gtwziogccu.html

[S32] C++：字符串
来源：http://hz.hfpthk.cn/gtdmnsfewu.html

std::string s = "hi";  s += "!";
来源：http://hz.gogol.net.cn/gtgvbwbqty.html

[S33] C++：vector 增删
来源：http://hz.feifeiyinyue.top/gtuhnvphyw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xylfe.cn/gthrydoswr.html

[S34] C++：遍历 vector
来源：http://hz.sysykeji.top/gtxgvvqahv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gaohongyu789.top/gtxhmajtmz.html

[S35] C++：map
来源：http://hz.hfpthk.cn/gterdrrvbj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gtwxdntspn.html

[S36] C++：unordered_map
来源：http://hz.fengsongda.top/gtjhiydqnj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtfzdftnnb.html

[S37] C++：set
来源：http://hz.dianchejie.cn/gtvxxkqkvq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.pycfn.com/gtqcoulfow.html

[S38] C++：排序
来源：http://hz.hammf.cn/gtcsrkjiuw.html

std::sort(v.begin(), v.end());
来源：http://hz.0kj1m.cn/gtjiipjaxd.html

[S39] C++：自定义比较器排序
来源：http://hz.andypj.xyz/gtacfvvebd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gotoacloud.top/gtazclrfbh.html

[S40] C++：查找元素
来源：http://hz.yueranfly.top/gtismzvvto.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sufxvd.cn/gtqarnypmg.html

[S41] C++：类与构造函数
来源：http://hz.zdqjudy.top/gtxqfkeqyi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.meibo888.top/gtkbfcijwv.html

[S42] C++：继承与虚函数
来源：http://hz.gaohongyu789.top/gtdommszoq.html

class B : public Base { public: void f() override {} };
来源：http://hz.cucudq.cn/gtjwmuhzyx.html

[S43] C++：智能指针
来源：http://hz.ydjk.org.cn/gtulygytio.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhongyouzk.top/gtzwhzveqo.html

[S44] C++：引用传参
来源：http://hz.jinghuilouyu.cn/gtouzqffjo.html

void inc(int &x) { ++x; }
来源：http://hz.guowangkeji.top/gtjpgqzmtp.html

[S45] C++：lambda
来源：http://hz.pycfn.com/gtuhvgbejo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xingfuxueyuan.xyz/gtuvqmjsvp.html

[S46] C++：函数模板
来源：http://hz.quarkkingdee.top/gtivsyancs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.c1oappe.top/gtbdzkpnak.html

[S47] C++：结构化绑定遍历
来源：http://hz.yuxming.cn/gtcokgxsaa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ydjk.org.cn/gthsvilfxv.html

[S48] C++：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtzcpqvber.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.smart0.xyz/gtbvrvqzsk.html

while (std::getline(in, line)) { }
来源：http://hz.ivvv.top/gtympwiokf.html

[S49] C++：写文件
来源：http://hz.yuanzhike.top/gtntazvkra.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnxiangtu.top/gtxcwqcxuj.html

[S50] C++：格式化数字
来源：http://hz.hywenlv.cn/gtsxkdxpwc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ppjwa.cn/gtpchhhpay.html

[S51] C++：显式类型转换
来源：http://hz.cqqwz.cn/gtauqwzert.html

static_cast<double>(a) / b
来源：http://hz.zhiwuduotai.top/gtnkjjdxkm.html

[S52] C++：const 与 noexcept
来源：http://hz.yueranfly.top/gtniguelmq.html

int size() const noexcept { return n_; }
来源：http://hz.zhiwuduotai.top/gtajbuzxzw.html

[S53] C++：移动语义
来源：http://hz.zhixingplan.top/gtixpzkfeo.html

std::vector<int> w = std::move(v);
来源：http://hz.zhiwuduotai.top/gtjllsjyff.html

[S54] C++：异常处理
来源：http://hz.jqgufenzy.top/gtztpwkejc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj202588.top/gtvttrdfzx.html

[S55] C++：结构化绑定
来源：http://hz.shuidangran.top/gtdlyqaika.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.0kj1m.cn/gthxwoqfeo.html

[S56] C++：optional
来源：http://hz.chenlongwang.top/gtxmfltxxd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hammf.cn/gtecdmdmhz.html

[S57] C++：编译期常量
来源：http://hz.hywenlv.cn/gtvynbhgcz.html

constexpr int N = 10;
来源：http://hz.fzhhl.top/gtjbxrhifx.html

[S58] C++：命名空间
来源：http://hz.yuxming.cn/gtseuacduh.html

namespace ns { int f() { return 1; } }
来源：http://hz.9152youxi.cn/gtuiuplmvh.html

[S59] C++：静态断言
来源：http://hz.dashuyun.cn/gtgtxxglwn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.dianchejie.cn/gtbxleatqz.html

[S60] C++：遍历并删除元素
来源：http://hz.zhijiandao.cn/gtwamlqgqj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhijiandao.cn/gtcmjbblmd.html

================================================================================
来源：http://hz.sufxvd.cn/gthavgfmwn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xziqi.cn/gtfjfwyvjl.html

================================================================================
来源：http://hz.iojbl.cn/gtmfyuwqib.html

[T01] Kotlin：Hello World
来源：http://hz.c1oappe.top/gtblielgih.html

println("Hello")
来源：http://hz.feifeiyinyue.top/gtwgufxbyh.html

[T02] Kotlin：变量
来源：http://hz.chenlongwang.top/gtrbcilgtb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tian-w.cn/gtxjeqibpb.html

[T03] Kotlin：字符串模板
来源：http://hz.ydjk.org.cn/gtcosreyby.html

"值: $b"
来源：http://hz.chenlongwang.top/gtjbpglagx.html

[T04] Kotlin：空安全
来源：http://hz.redwolf501.top/gtfpzjsqrn.html

val n: String? = null;  n?.length
来源：http://hz.sysykeji.top/gttptgxpqr.html

[T05] Kotlin：when 表达式
来源：http://hz.jqgufenzy.top/gtszwgjntk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhongyouzk.top/gtkxbcmutj.html

[T06] Kotlin：集合映射
来源：http://hz.andypj.xyz/gtmuzzmvwt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jqgfzy.top/gtggchudnn.html

[T07] Kotlin：集合过滤
来源：http://hz.shanyushiyangtech.top/gtpdnhuejs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinghuilouyu.cn/gtbqdygzmy.html

[T08] Kotlin：数据类
来源：http://hz.wangshuangyany.cn/gttbibpgng.html

data class User(val name: String, val age: Int)
来源：http://hz.hysaishi.cn/gtaogahaii.html

[T09] Kotlin：扩展函数
来源：http://hz.hammf.cn/gtttzhnqmz.html

fun String.exclaim() = this + "!"
来源：http://hz.ivvv.top/gttismmpaa.html

[T10] Kotlin：默认参数
来源：http://hz.yuanzhike.top/gtppnsugpe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aizwys.cn/gtolfrjuwq.html

[T11] Kotlin：协程
来源：http://hz.zdqjudy.top/gtayqmjerp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhengqikj.top/gtwrtztejw.html

[T12] Kotlin：解构声明
来源：http://hz.yonumen.top/gtwxubjutm.html

val (a, b) = Pair(1, 2)
来源：http://hz.jqgfzy.top/gtsqjrollh.html

[T13] Kotlin：只读 Map
来源：http://hz.9152youxi.cn/gtzlxpnwbt.html

val m = mapOf("a" to 1)
来源：http://hz.0kj1m.cn/gtpnqjrgko.html

[T14] Kotlin：循环
来源：http://hz.hnxiangtu.top/gtjpkzprcu.html

for (i in 1..10) println(i)
来源：http://hz.c1oappe.top/gtbrwrdeav.html

[T15] Kotlin：接口
来源：http://hz.pengpengdd.cyou/gtixkxcosc.html

interface Shape { fun area(): Double }
来源：http://hz.havefunace.top/gtqbuzacso.html

[T16] Swift：Hello World
来源：http://hz.cdnleiting.top/gtwljcjfec.html

print("Hello")
来源：http://hz.yangfankeji.com/gtcyjphetr.html

[T17] Swift：变量与常量
来源：http://hz.jlsjyb.cn/gtatcnhwwo.html

var a = 1;  let b = 2
来源：http://hz.yuxming.cn/gtaxtgjgew.html

[T18] Swift：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtzwnexepj.html

"值: \(b)"
来源：http://hz.fzhhl.top/gtqpcrggla.html

[T19] Swift：可选绑定
来源：http://hz.jinyuanbaomall.cn/gtqqivnhfh.html

if let n = opt { print(n) }
来源：http://hz.yanxiufei.cn/gtvufhgfss.html

[T20] Swift：数组操作
来源：http://hz.cashguo.top/gtfbnbrcwb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fengsongda.top/gtrhlqgahh.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gtbkwnxosa.html

for x in a { print(x) }
来源：http://hz.aibaodan.cn/gtststymwe.html

[T22] Swift：字典
来源：http://hz.tianlin.xyz/gtlcrarrdi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhaomingkeji.xyz/gthgdekkqh.html

[T23] Swift：函数
来源：http://hz.ehwqpu.com/gttfuwnhau.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sweek.top/gtzrvpzypm.html

[T24] Swift：闭包
来源：http://hz.ydzc1.top/gtlbzfroes.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.snrcjt.cn/gtlfjzdore.html

[T25] Swift：结构体
来源：http://hz.ppjwa.cn/gtsfillvhf.html

struct P { var x: Int }
来源：http://hz.hammf.cn/gtzauphyqf.html

[T26] Swift：类与重写
来源：http://hz.xuetiantiany.cn/gtzbjqbvyn.html

class A: Base { override func f() {} }
来源：http://hz.ydjk.org.cn/gtpllgpeae.html

[T27] Swift：错误处理
来源：http://hz.ppjwa.cn/gtqxftehbi.html

do { try f() } catch { print(error) }
来源：http://hz.wangshuangyany.cn/gtkxnamqey.html

[T28] Swift：枚举
来源：http://hz.jiagoushi.top/gtlvjcqwxd.html

enum Color { case red, green }
来源：http://hz.aizwys.cn/gtuabwloxy.html

[T29] Swift：guard 提前返回
来源：http://hz.c1oappe.top/gtzttowzvo.html

guard let x = opt else { return }
来源：http://hz.mhx1999.top/gtqcakfaws.html

[T30] Swift：协议
来源：http://hz.yuanzhike.top/gtoowmdykq.html

protocol Shape { func area() -> Double }
来源：http://hz.yangfankeji.com/gtzmykolgv.html

[T31] Lua：Hello World
来源：http://hz.nanxinkj.top/gtnqlfpkyv.html

print("Hello")
来源：http://hz.ydjk.org.cn/gtmzjvrqdg.html

[T32] Lua：局部变量
来源：http://hz.ydjk.org.cn/gtivmuotok.html

local a = 1
来源：http://hz.ivvv.top/gtsiayylkp.html

[T33] Lua：表（数组）
来源：http://hz.yj20258888.top/gtavpzmteb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sysykeji.top/gtscrdrpgi.html

[T34] Lua：遍历表
来源：http://hz.shanyushiyangtech.top/gthkqogubv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xylfe.cn/gtqnjrpnwm.html

[T35] Lua：字典表
来源：http://hz.yvedp.cn/gtnvnueeuz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yueranfly.top/gtfmbmyenb.html

[T36] Lua：函数
来源：http://hz.hnqzz.top/gtnenclgrw.html

function add(a, b) return a + b end
来源：http://hz.cdnleiting.top/gtwoeerlew.html

[T37] Lua：字符串拼接
来源：http://hz.iojbl.cn/gtgjgmcdaf.html

"a" .. "b"
来源：http://hz.xuetiantiany.cn/gtvbbvxibm.html

[T38] Lua：条件
来源：http://hz.9152youxi.cn/gthpzbqktc.html

if x > 0 then print("正") end
来源：http://hz.sxryk.cn/gtbwsnkxta.html

[T39] Lua：模式匹配
来源：http://hz.tanke756.top/gtsropnojl.html

string.find(s, "%d+")
来源：http://hz.xinyue.icu/gturaresyk.html

[T40] Lua：元表
来源：http://hz.yueranfly.top/gtimyduxqg.html

setmetatable({}, { __index = base })
来源：http://hz.hammf.cn/gthqzmbfsy.html

[T41] Perl：Hello World
来源：http://hz.gotoacloud.top/gtgnofbzdx.html

print "Hello\n";
来源：http://hz.chenjidiqi.icu/gtggomnbwy.html

[T42] Perl：变量类型
来源：http://hz.andypj.xyz/gtccddctfl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinqigufen.top/gtobvfyrdb.html

[T43] Perl：字符串插值
来源：http://hz.hongshengwenyu.top/gtdxdoypwu.html

"值: $a"
来源：http://hz.dianchejie.cn/gtplddcdxh.html

[T44] Perl：条件
来源：http://hz.yj20258.top/gtknpyjdxp.html

if ($a > 0) { print "正"; }
来源：http://hz.cheryme.top/gthaqtdein.html

[T45] Perl：数组遍历
来源：http://hz.zhiwuduotai.top/gtboqkmgel.html

for my $x (@arr) { print $x; }
来源：http://hz.xuanzx.com/gttzrltvtc.html

[T46] Perl：哈希操作
来源：http://hz.zycfv.cn/gtxdhfqypw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hnqzz.top/gtsgqlsuyz.html

[T47] Perl：正则捕获
来源：http://hz.dianchejie.cn/gtudkosiqg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shzxlz.cn/gtwfkehwsd.html

[T48] Perl：正则替换
来源：http://hz.redwolf501.top/gtufxjjfby.html

$s =~ s/old/new/g;
来源：http://hz.ybcxt.top/gtvrboovgt.html

[T49] Perl：函数
来源：http://hz.fzhhl.top/gtawopvzbo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gotoacloud.top/gtiihfzysc.html

[T50] Perl：逐行读文件
来源：http://hz.daria6918.cn/gtpchpcsdg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sweek.top/gtyvecniso.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yonumen.top/gtclsqvasi.html

[T51] Scala：Hello World
来源：http://hz.snrcjt.cn/gttkbmnphv.html

println("Hello")
来源：http://hz.chenlongwang.top/gtokcyiovs.html

[T52] Scala：变量
来源：http://hz.yueranfly.top/gtwudfofte.html

val a = 1;  var b = 2
来源：http://hz.gotoacloud.top/gtkxpzkhjs.html

[T53] Scala：字符串插值
来源：http://hz.zycfv.cn/gtqfisyavg.html

s"值: $b"
来源：http://hz.c1oappe.top/gtekuyjhqk.html

[T54] Scala：集合映射
来源：http://hz.iojbl.cn/gtxvvfhfic.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.mhx1999.top/gtkzkliuwa.html

[T55] Scala：集合过滤
来源：http://hz.ppjwa.cn/gtswpnpmvk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.fengsongda.top/gtknrgydci.html

[T56] Scala：样例类
来源：http://hz.sufxvd.cn/gtedkjonxn.html

case class User(name: String, age: Int)
来源：http://hz.jlsjyb.cn/gtncmwhkpk.html

[T57] Scala：模式匹配
来源：http://hz.jqgfzy.top/gtwdgnmvdv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xinyue.icu/gtpscgjkhx.html

[T58] Scala：函数定义
来源：http://hz.ydzc1.top/gtlnfojaba.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.tanke756.top/gtnludggik.html

[T59] Scala：循环
来源：http://hz.316326.xyz/gtihhkqhhj.html

for (i <- 1 to 10) println(i)
来源：http://hz.ybcxt.top/gtwuefadex.html

[T60] Scala：折叠
来源：http://hz.zycfv.cn/gtwwauanqa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chenzaomai.com/gtfqtilzhf.html

================================================================================
来源：http://hz.0kj1m.cn/gtlgfryksd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxuanxn.top/gtskulqjxe.html

================================================================================
来源：http://hz.yj202588.top/gtialrigim.html

[U01] Py：创建虚拟环境
来源：http://hz.yuxming.cn/gtggbvlxgw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.snrcjt.cn/gtreymgyxe.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhijiandao.cn/gthqmbxcdy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gogol.net.cn/gttulweefs.html

[U03] Py：加载 .env 配置
来源：http://hz.pengpengdd.cyou/gtrhthzeju.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.wangshuangyany.cn/gtakmgublw.html

[U04] Py：变量调试打印
来源：http://hz.andypj.xyz/gtthvyklbx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhixingplan.top/gtyvosleqe.html

[U05] Py：列表去重且保序
来源：http://hz.yj20258888.top/gtgffjykbo.html

list(dict.fromkeys(arr))
来源：http://hz.hnqzz.top/gtsvvwmslm.html

[U06] Py：合并两个字典
来源：http://hz.iojbl.cn/gtpfnbubly.html

{**a, **b}
来源：http://hz.pengpengdd.cyou/gtwitenblu.html

[U07] Py：反转字典键值
来源：http://hz.shangyingyoupin.top/gtwgyajehq.html

{v: k for k, v in d.items()}
来源：http://hz.9152youxi.cn/gtebwxdotm.html

[U08] Py：展平二维列表
来源：http://hz.zhaomingkeji.xyz/gtzewdtdpq.html

[y for x in nested for y in x]
来源：http://hz.sysykeji.top/gtdowyqelm.html

[U09] Py：字典取最大值的键
来源：http://hz.dashuyun.cn/gtkzflynes.html

max(d, key=d.get)
来源：http://hz.iojbl.cn/gtafpgwsay.html

[U10] Py：按值排序字典
来源：http://hz.xuanzx.com/gtgytxzkeb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yanxiufei.cn/gtilsjucas.html

[U11] Py：生成器表达式
来源：http://hz.xziqi.cn/gtnnifpdga.html

(x * 2 for x in arr)
来源：http://hz.gotoacloud.top/gtjuajpgir.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xziqi.cn/gturwsyqzb.html

Counter(arr).most_common(3)
来源：http://hz.chenzaomai.com/gtoktzgkeb.html

[U13] Py：固定长度队列
来源：http://hz.cashguo.top/gtjfivzshk.html

deque(maxlen=10)
来源：http://hz.ydzc1.top/gtpshudplv.html

[U14] Py：分组收集到列表
来源：http://hz.fzhhl.top/gtesaajrax.html

defaultdict(list)
来源：http://hz.dianchejie.cn/gtiregnwqn.html

[U15] Py：高精度计时
来源：http://hz.shanyushiyangkeji.top/gtpqudxvgg.html

t = time.perf_counter()
来源：http://hz.yangfankeji.com/gtefclgtwu.html

[U16] Py：命令行参数解析
来源：http://hz.jyoumei.cn/gtuukkbddo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yuanzhike.top/gtgakmrszr.html

[U17] Py：初始化日志
来源：http://hz.gzhubu.top/gtbobuhokj.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.andypj.xyz/gtsprlmmff.html

[U18] Py：预编译正则
来源：http://hz.nanxuanxn.top/gtdusepstl.html

pat = re.compile(r"\d+")
来源：http://hz.andypj.xyz/gtvhvbdywo.html

[U19] Py：正则替换带回调
来源：http://hz.daxiang520.top/gtixjunhow.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xuetiantiany.cn/gtvujxsbiy.html

[U20] Py：缓存函数结果
来源：http://hz.birdmap.top/gtqfcmirol.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj202588.top/gtkfozldtk.html

[U21] Py：自定义上下文管理器
来源：http://hz.xziqi.cn/gtolediogj.html

@contextlib.contextmanager
来源：http://hz.hywenlv.cn/gtlmkmhtwz.html

[U22] Py：矩阵转置
来源：http://hz.gotoacloud.top/gtdfokbmzd.html

list(zip(*m))
来源：http://hz.tianlin.xyz/gtvthtcpxb.html

[U23] Py：分块读取大文件
来源：http://hz.jinyuanbaomall.cn/gteghjcsno.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cdnleiting.top/gtisjkqchl.html

[U24] Py：路径操作
来源：http://hz.yueranfly.top/gtauskcint.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ydzc1.top/gtgtjketeb.html

[U25] Py：CSV 按字典读
来源：http://hz.hysaishi.cn/gtdfdgxqxg.html

csv.DictReader(f)
来源：http://hz.ybcxt.top/gtfxhjxktj.html

[U26] Py：并发下载
来源：http://hz.c1oappe.top/gtbailkrka.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.quarkkingdee.top/gtxpjhnrni.html

[U27] Py：异步 HTTP
来源：http://hz.c1oappe.top/gtcebhuweg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.snrcjt.cn/gtxkvwsxjq.html

[U28] Py：类型别名
来源：http://hz.snrcjt.cn/gtyozrlnei.html

UserId = int
来源：http://hz.aibaodan.cn/gtwbgikcjb.html

[U29] Py：属性校验
来源：http://hz.jinqigufen.top/gtlvgnnryz.html

@property 与 @x.setter 配合
来源：http://hz.yangfankeji.com/gtuzvxirnn.html

[U30] Py：数据类
来源：http://hz.xuetiantiany.cn/gtjtzreahn.html

@dataclass(slots=True)
来源：http://hz.aibaodan.cn/gtsghjwgbh.html

[U31] Py：单测
来源：http://hz.hywenlv.cn/gtklniwuck.html

python -m pytest -q
来源：http://hz.zhoulong.xyz/gtemhsggkg.html

[U32] Py：代码格式化
来源：http://hz.nanxinkj.top/gtigxpfqsv.html

ruff format . && ruff check --fix .
来源：http://hz.zhiwuduotai.top/gtckwwdqis.html

[U33] Py：打包发布
来源：http://hz.tanke756.top/gtvrxkgayk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yangfankeji.com/gtuxjyvslu.html

[U34] Py：判断编码
来源：http://hz.jlsjyb.cn/gtijhfgpyk.html

chardet.detect(raw)
来源：http://hz.zhongyouzk.top/gtvkyczxpp.html

[U35] Py：发送邮件
来源：http://hz.cucudq.cn/gtuqzprlrr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.guannengcc.top/gtkmbkbvyk.html

[U36] Py：定时任务
来源：http://hz.xylfe.cn/gtrvqnaepp.html

schedule.every(10).minutes.do(job)
来源：http://hz.jinghuilouyu.cn/gtquhgbxhg.html

[U37] Py：读写 Excel
来源：http://hz.hfpthk.cn/gtuxxjrvpy.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.52xcode.cn/gtawofrvua.html

[U38] Py：获取脚本所在目录
来源：http://hz.9152youxi.cn/gtgwubzfro.html

Path(__file__).resolve().parent
来源：http://hz.gotoacloud.top/gtspkjsprl.html

[U39] Py：判断是否在交互环境
来源：http://hz.tanke756.top/gtgwkghkxk.html

sys.stdout.isatty()
来源：http://hz.smart0.xyz/gtpvaipldd.html

[U40] Py：打印到标准错误
来源：http://hz.nwbrower.top/gtezeaedhi.html

print("err", file=sys.stderr)
来源：http://hz.gotoacloud.top/gtmnhovbpv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenjidiqi.icu/gtziavktuw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cdnleiting.top/gtvmwrcqbo.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.dianchejie.cn/gtdqhmqbwe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yuxming.cn/gtmlpvjmuj.html

[U43] PHP：声明命名空间
来源：http://hz.c1oappe.top/gtnlmnzztu.html

namespace App\Http;
来源：http://hz.gotoacloud.top/gtebuuysjn.html

[U44] PHP：开启严格类型
来源：http://hz.aizwys.cn/gtogjhqwun.html

declare(strict_types=1);
来源：http://hz.fzhhl.top/gtznvtpjnk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xziqi.cn/gtsdocwkrj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtrfnbjjwc.html

[U46] PHP：可空类型
来源：http://hz.vqdsnc.cn/gtgvcupnom.html

?string $name = null
来源：http://hz.zhixingplan.top/gtyjblgoua.html

[U47] PHP：联合类型
来源：http://hz.zhaomingkeji.xyz/gtzgukhjag.html

int|string $id
来源：http://hz.shuidangran.top/gtbtsajbgm.html

[U48] PHP：纯枚举
来源：http://hz.pycfn.com/gtztmdyntj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.pengpengdd.cyou/gtpkxvxlyp.html

[U49] PHP：只读属性
来源：http://hz.sysykeji.top/gtgqwrervh.html

public readonly string $name
来源：http://hz.fzhhl.top/gtyvihjbfk.html

[U50] PHP：构造器属性提升
来源：http://hz.yueranfly.top/gttzwgnibr.html

public function __construct(private int $id) {}
来源：http://hz.shanyushiyangkeji.top/gtxynpmgsn.html

[U51] PHP：数组解构
来源：http://hz.yj202588.top/gtubnsuxeo.html

[$a, $b] = $arr;
来源：http://hz.jiagoushi.top/gtusafjuqa.html

[U52] PHP：箭头函数
来源：http://hz.snrcjt.cn/gtwvxjhvvm.html

$double = fn($x) => $x * 2;
来源：http://hz.cdnleiting.top/gtoiwvilos.html

[U53] PHP：空合并运算符
来源：http://hz.chenlongwang.top/gtcwbppjjp.html

$v = $a ?? $b ?? "default";
来源：http://hz.gotoacloud.top/gttpxfkeqw.html

[U54] PHP：空安全调用
来源：http://hz.chenlongwang.top/gtxaprgcbl.html

$obj?->method()
来源：http://hz.hysaishi.cn/gtbopxdzkp.html


<!-- 参考信息 -->