代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jiagoushi.top/gtpfwrihla.html

[S25] C：内存拷贝
来源：http://hz.nwbrower.top/gtshjdyuvw.html

memcpy(dst, src, n);
来源：http://hz.fengsongda.top/gtmhrttiyk.html

[S26] C：内存清零
来源：http://hz.dianchejie.cn/gtxxuhkvgp.html

memset(a, 0, sizeof a);
来源：http://hz.hongshengwenyu.top/gtoilrnbfp.html

[S27] C：定义常量
来源：http://hz.hnqzz.top/gtfjuvupka.html

const double PI = 3.14159;
来源：http://hz.yvedp.cn/gtidzmpnoa.html

[S28] C：静态变量
来源：http://hz.zhongyouzk.top/gtsptjmbgb.html

static int counter = 0;
来源：http://hz.hfpthk.cn/gtyycyoaor.html

[S29] C：变参函数
来源：http://hz.cdnleiting.top/gttacgvpuv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gotoacloud.top/gtxaddnylf.html

[S30] C：头文件保护
来源：http://hz.nwbrower.top/gtfejypeqw.html

#ifndef X_H
来源：http://hz.andypj.xyz/gtrfmeidow.html

#define X_H
来源：http://hz.xuetiantiany.cn/gtunejmewo.html

#endif
来源：http://hz.ppjwa.cn/gtpwrcegdi.html

[S31] C++：Hello World
来源：http://hz.yvedp.cn/gtdzmvacsq.html

#include <iostream>
来源：http://hz.316326.xyz/gtyuctcqmy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sxryk.cn/gtumdavrcc.html

[S32] C++：字符串
来源：http://hz.c1oappe.top/gtbqfdqmhg.html

std::string s = "hi";  s += "!";
来源：http://hz.gogol.net.cn/gtgdwtwpwv.html

[S33] C++：vector 增删
来源：http://hz.zhongyouzk.top/gtbsoxkrmr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xuanzx.com/gtlytsfhvb.html

[S34] C++：遍历 vector
来源：http://hz.zhengqikj.top/gtnlefaoap.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ybcxt.top/gttrylvfix.html

[S35] C++：map
来源：http://hz.aizwys.cn/gtlxjufhsl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.haohaochexian.top/gtfphyybks.html

[S36] C++：unordered_map
来源：http://hz.hnxiangtu.top/gtqdnrfdum.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuetiantiany.cn/gtuicdxxaz.html

[S37] C++：set
来源：http://hz.yuanzhike.top/gtisykhhcn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnqzz.top/gtinlcjhke.html

[S38] C++：排序
来源：http://hz.hnxiangtu.top/gtssktrvxy.html

std::sort(v.begin(), v.end());
来源：http://hz.sysykeji.top/gtfrhyqriv.html

[S39] C++：自定义比较器排序
来源：http://hz.zhoulong.xyz/gtdywbiysd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dianchejie.cn/gtzpfncmvo.html

[S40] C++：查找元素
来源：http://hz.jianghu66.top/gtvebpxdby.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinqigfzy.top/gttyyjxbsr.html

[S41] C++：类与构造函数
来源：http://hz.wangshuangyany.cn/gtzsgrflft.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.kuanghao11.cn/gtrgxbzplj.html

[S42] C++：继承与虚函数
来源：http://hz.gotoacloud.top/gtfhnsrjkw.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinyuanbaomall.cn/gtqoyjlqqb.html

[S43] C++：智能指针
来源：http://hz.hfpthk.cn/gtyapnvtdo.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxuanxn.top/gtdsejmqxf.html

[S44] C++：引用传参
来源：http://hz.jqgfzy.top/gtxfltcmye.html

void inc(int &x) { ++x; }
来源：http://hz.ydjk.org.cn/gtcmwtixio.html

[S45] C++：lambda
来源：http://hz.meibo888.top/gtqkwsablo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.daxiang520.top/gtccdfuzor.html

[S46] C++：函数模板
来源：http://hz.tian-w.cn/gtjgkqpvop.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.iojbl.cn/gtajjtorxh.html

[S47] C++：结构化绑定遍历
来源：http://hz.gaohongyu789.top/gtdokpubze.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinqigufen.top/gtxxibiwlu.html

[S48] C++：逐行读文件
来源：http://hz.gogol.net.cn/gtnyraogxv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xuanzx.com/gtxncvxauw.html

while (std::getline(in, line)) { }
来源：http://hz.xinyue.icu/gtttybpnti.html

[S49] C++：写文件
来源：http://hz.cheryme.top/gtaorcfqgk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhongyouzk.top/gtizibexkn.html

[S50] C++：格式化数字
来源：http://hz.ppjwa.cn/gtxmkuodtn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigufen.top/gtdvtpeqhm.html

[S51] C++：显式类型转换
来源：http://hz.aibaodan.cn/gtafprpbyu.html

static_cast<double>(a) / b
来源：http://hz.chenzaomai.com/gtvidsktxd.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258888.top/gtlugoacni.html

int size() const noexcept { return n_; }
来源：http://hz.fzhhl.top/gtipiyiipd.html

[S53] C++：移动语义
来源：http://hz.jqgufenzy.top/gtoudbckfm.html

std::vector<int> w = std::move(v);
来源：http://hz.cashguo.top/gteecgqted.html

[S54] C++：异常处理
来源：http://hz.zhixingplan.top/gtbzdpeyno.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ybcxt.top/gtskxcyjja.html

[S55] C++：结构化绑定
来源：http://hz.yj202588.top/gteudgmwmc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gotoacloud.top/gtsjenybdg.html

[S56] C++：optional
来源：http://hz.sufxvd.cn/gtkppsplxe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guowangkeji.top/gtzepxuveo.html

[S57] C++：编译期常量
来源：http://hz.cdnleiting.top/gtqortiwsu.html

constexpr int N = 10;
来源：http://hz.yongpay.top/gtubxwazum.html

[S58] C++：命名空间
来源：http://hz.sweek.top/gtlxstxqch.html

namespace ns { int f() { return 1; } }
来源：http://hz.cucudq.cn/gtwflexblg.html

[S59] C++：静态断言
来源：http://hz.tianlin.xyz/gtrzhqhvoj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sxryk.cn/gtarsauysc.html

[S60] C++：遍历并删除元素
来源：http://hz.redwolf501.top/gtlmrptfxp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jianghu66.top/gteohgxmfn.html

================================================================================
来源：http://hz.aizwys.cn/gttrvoucry.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jiagoushi.top/gtzjfvetgp.html

================================================================================
来源：http://hz.dianchejie.cn/gtwxaaxery.html

[T01] Kotlin：Hello World
来源：http://hz.yonumen.top/gteaorosrq.html

println("Hello")
来源：http://hz.wangdashe.top/gtoxmcqxvs.html

[T02] Kotlin：变量
来源：http://hz.xingfuxueyuan.xyz/gtktxuaqwd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yuanzhike.top/gtismynjhl.html

[T03] Kotlin：字符串模板
来源：http://hz.chenzaomai.com/gtodxsuopy.html

"值: $b"
来源：http://hz.daria6918.cn/gtphyojcnw.html

[T04] Kotlin：空安全
来源：http://hz.andypj.xyz/gtgvbjjvmy.html

val n: String? = null;  n?.length
来源：http://hz.bjfxy.top/gtpggtltln.html

[T05] Kotlin：when 表达式
来源：http://hz.daxiang520.top/gtwvrwmmee.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zycfv.cn/gtooipdyug.html

[T06] Kotlin：集合映射
来源：http://hz.xuetiantiany.cn/gtwpsywibg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sxryk.cn/gtpmmpudoz.html

[T07] Kotlin：集合过滤
来源：http://hz.xziqi.cn/gttjbykcpg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.andypj.xyz/gtqgpijiqh.html

[T08] Kotlin：数据类
来源：http://hz.jinqigfzy.top/gtfxnhtjny.html

data class User(val name: String, val age: Int)
来源：http://hz.hnxiangtu.top/gtwrqpiavg.html

[T09] Kotlin：扩展函数
来源：http://hz.zhixingplan.top/gtobnkmhvi.html

fun String.exclaim() = this + "!"
来源：http://hz.chenzaomai.com/gtmrntzgid.html

[T10] Kotlin：默认参数
来源：http://hz.jiagoushi.top/gtfpgbwiae.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigufen.top/gtmflaonzp.html

[T11] Kotlin：协程
来源：http://hz.ybcxt.top/gtwhkatwxs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shangyingyoupin.top/gttqrxkkda.html

[T12] Kotlin：解构声明
来源：http://hz.zhoulong.xyz/gtyhkltwmy.html

val (a, b) = Pair(1, 2)
来源：http://hz.havefunace.top/gtummiugtf.html

[T13] Kotlin：只读 Map
来源：http://hz.ydzc1.top/gtofmnegvq.html

val m = mapOf("a" to 1)
来源：http://hz.vqdsnc.cn/gtkrzwfdmv.html

[T14] Kotlin：循环
来源：http://hz.yangfankeji.com/gtlyojbong.html

for (i in 1..10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtthidddvp.html

[T15] Kotlin：接口
来源：http://hz.aizwys.cn/gtyiftsjba.html

interface Shape { fun area(): Double }
来源：http://hz.chenjidiqi.icu/gteltmxdnx.html

[T16] Swift：Hello World
来源：http://hz.guannengcc.top/gtbnyhxmqc.html

print("Hello")
来源：http://hz.guannengcc.top/gtfkjqodbe.html

[T17] Swift：变量与常量
来源：http://hz.hysaishi.cn/gtcmyobmpp.html

var a = 1;  let b = 2
来源：http://hz.zhoulong.xyz/gtyvjyitec.html

[T18] Swift：字符串插值
来源：http://hz.sufxvd.cn/gtcwzzqqkh.html

"值: \(b)"
来源：http://hz.chenjidiqi.icu/gtciwyrgvl.html

[T19] Swift：可选绑定
来源：http://hz.316326.xyz/gtrummdxzi.html

if let n = opt { print(n) }
来源：http://hz.wangdashe.top/gtpslamjzo.html

[T20] Swift：数组操作
来源：http://hz.jyoumei.cn/gtgdmevnfa.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jyoumei.cn/gtogonpyfv.html

[T21] Swift：遍历
来源：http://hz.quarkkingdee.top/gtphtksmqg.html

for x in a { print(x) }
来源：http://hz.guowangkeji.top/gtjzvekjsg.html

[T22] Swift：字典
来源：http://hz.zhengqikj.top/gtcldqjwuc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tian-w.cn/gtldayaqrg.html

[T23] Swift：函数
来源：http://hz.daria6918.cn/gtiprgqxeq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ydzc1.top/gtxvybblzd.html

[T24] Swift：闭包
来源：http://hz.redwolf501.top/gtfdlduxnl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.fengsongda.top/gtxrnyrpza.html

[T25] Swift：结构体
来源：http://hz.9152youxi.cn/gtcgnnrlyf.html

struct P { var x: Int }
来源：http://hz.ywan-chungtsiang.top/gtxnkbtwyl.html

[T26] Swift：类与重写
来源：http://hz.cashguo.top/gtzaibhvmm.html

class A: Base { override func f() {} }
来源：http://hz.ppjwa.cn/gtddblaztm.html

[T27] Swift：错误处理
来源：http://hz.sysykeji.top/gttdciamme.html

do { try f() } catch { print(error) }
来源：http://hz.gzhubu.top/gttcibzppt.html

[T28] Swift：枚举
来源：http://hz.hammf.cn/gtbcpyivqo.html

enum Color { case red, green }
来源：http://hz.ppjwa.cn/gtoncdpxvj.html

[T29] Swift：guard 提前返回
来源：http://hz.vqdsnc.cn/gtjxxdpqnr.html

guard let x = opt else { return }
来源：http://hz.yueranfly.top/gtyjfqmptg.html

[T30] Swift：协议
来源：http://hz.guowangkeji.top/gtqhamjbcq.html

protocol Shape { func area() -> Double }
来源：http://hz.jianghu66.top/gtasroqlyq.html

[T31] Lua：Hello World
来源：http://hz.smart0.xyz/gtbtpgfhrv.html

print("Hello")
来源：http://hz.tianlin.xyz/gttjhuacki.html

[T32] Lua：局部变量
来源：http://hz.zhiwuduotai.top/gtvoedhnwa.html

local a = 1
来源：http://hz.redwolf501.top/gtchdqjxzj.html

[T33] Lua：表（数组）
来源：http://hz.daxiang520.top/gtjrpgftvd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.meibo888.top/gtlknhmrpo.html

[T34] Lua：遍历表
来源：http://hz.tianlin.xyz/gtdwbvhdsf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ehwqpu.com/gttsfzytsn.html

[T35] Lua：字典表
来源：http://hz.shzxlz.cn/gtlfpcairq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.snrcjt.cn/gtixvgdgel.html

[T36] Lua：函数
来源：http://hz.nanxinkj.top/gtmnqlafez.html

function add(a, b) return a + b end
来源：http://hz.iojbl.cn/gtwhcytuax.html

[T37] Lua：字符串拼接
来源：http://hz.zhixingplan.top/gtsaodmotr.html

"a" .. "b"
来源：http://hz.redwolf501.top/gtykfddaye.html

[T38] Lua：条件
来源：http://hz.316326.xyz/gtoqgevolx.html

if x > 0 then print("正") end
来源：http://hz.shanyushiyangkeji.top/gtfmhsrzty.html

[T39] Lua：模式匹配
来源：http://hz.wangdashe.top/gtkkscogyg.html

string.find(s, "%d+")
来源：http://hz.cashguo.top/gtzhuhhbvj.html

[T40] Lua：元表
来源：http://hz.zhoulong.xyz/gtealgqtwj.html

setmetatable({}, { __index = base })
来源：http://hz.chenjidiqi.icu/gtmdxshssr.html

[T41] Perl：Hello World
来源：http://hz.nanxuanxn.top/gtofxidqac.html

print "Hello\n";
来源：http://hz.dashuyun.cn/gtyaabqqok.html

[T42] Perl：变量类型
来源：http://hz.cdnleiting.top/gtsypummct.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gogol.net.cn/gtliiqdlzl.html

[T43] Perl：字符串插值
来源：http://hz.cucudq.cn/gtbcwtuuzl.html

"值: $a"
来源：http://hz.zhongyouzk.top/gtplkxnnxw.html

[T44] Perl：条件
来源：http://hz.svipenyu.cn/gtgdsmqozg.html

if ($a > 0) { print "正"; }
来源：http://hz.xinyue.icu/gttxsyhszj.html

[T45] Perl：数组遍历
来源：http://hz.fzhhl.top/gtjwegddtk.html

for my $x (@arr) { print $x; }
来源：http://hz.quarkkingdee.top/gtqtrrkzby.html

[T46] Perl：哈希操作
来源：http://hz.shanyushiyangtech.top/gtbsnfjtqw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yongpay.top/gtgqfsrodz.html

[T47] Perl：正则捕获
来源：http://hz.nanxinkj.top/gtifltxjjh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shangyingyoupin.top/gtdnhrenfr.html

[T48] Perl：正则替换
来源：http://hz.dianchejie.cn/gtihvmdroi.html

$s =~ s/old/new/g;
来源：http://hz.andypj.xyz/gtxyaoiagq.html

[T49] Perl：函数
来源：http://hz.hnxiangtu.top/gtnredkomd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.haohaochexian.top/gtifrcyola.html

[T50] Perl：逐行读文件
来源：http://hz.52xcode.cn/gtvqtfeidn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yongpay.top/gthyekvxme.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gogol.net.cn/gtuuhjzjcw.html

[T51] Scala：Hello World
来源：http://hz.chenlongwang.top/gttlvfhuac.html

println("Hello")
来源：http://hz.dianchejie.cn/gtteasznan.html

[T52] Scala：变量
来源：http://hz.jyoumei.cn/gtmswlfpgi.html

val a = 1;  var b = 2
来源：http://hz.yuanzhike.top/gtzvmllivr.html

[T53] Scala：字符串插值
来源：http://hz.wangdashe.top/gttwxdofgr.html

s"值: $b"
来源：http://hz.jinghuilouyu.cn/gtdrvciojn.html

[T54] Scala：集合映射
来源：http://hz.hfpthk.cn/gtxkwyklli.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.fengsongda.top/gttjflmxks.html

[T55] Scala：集合过滤
来源：http://hz.yuxming.cn/gtteafpqxw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhijiandao.cn/gtjmcytcet.html

[T56] Scala：样例类
来源：http://hz.svipenyu.cn/gtooqomoiy.html

case class User(name: String, age: Int)
来源：http://hz.ybcxt.top/gtmpkldcov.html

[T57] Scala：模式匹配
来源：http://hz.chenlongwang.top/gtgjtlostv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.c1oappe.top/gtvnodmdce.html

[T58] Scala：函数定义
来源：http://hz.cashguo.top/gtojovdfdt.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.tian-w.cn/gtldqyxffm.html

[T59] Scala：循环
来源：http://hz.jinqigfzy.top/gtkzygcmra.html

for (i <- 1 to 10) println(i)
来源：http://hz.gaohongyu789.top/gtefxrlfod.html

[T60] Scala：折叠
来源：http://hz.shanyushiyangtech.top/gtamydmwfb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinqigfzy.top/gtcbwbpewd.html

================================================================================
来源：http://hz.aizwys.cn/gtjfhziilr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.snrcjt.cn/gtazqefowu.html

================================================================================
来源：http://hz.gzhubu.top/gtjjpynjyq.html

[U01] Py：创建虚拟环境
来源：http://hz.shangyingyoupin.top/gtatrbhzix.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ybcxt.top/gtiedulmhc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ydjk.org.cn/gtpokahqku.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ydzc1.top/gtouesjvwu.html

[U03] Py：加载 .env 配置
来源：http://hz.xziqi.cn/gthtloimcx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tanke756.top/gtrznxkbjj.html

[U04] Py：变量调试打印
来源：http://hz.0kj1m.cn/gtpzjmpvat.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhaomingkeji.xyz/gtpemtxtik.html

[U05] Py：列表去重且保序
来源：http://hz.yanxiufei.cn/gtrfaewcqd.html

list(dict.fromkeys(arr))
来源：http://hz.chenlongwang.top/gtzblknpny.html

[U06] Py：合并两个字典
来源：http://hz.hammf.cn/gtqdqalktj.html

{**a, **b}
来源：http://hz.zhaomingkeji.xyz/gtrrlqksau.html

[U07] Py：反转字典键值
来源：http://hz.feifeiyinyue.top/gtmyjcflty.html

{v: k for k, v in d.items()}
来源：http://hz.ivvv.top/gtiiumxkbz.html

[U08] Py：展平二维列表
来源：http://hz.yanxiufei.cn/gtrzipnbbg.html

[y for x in nested for y in x]
来源：http://hz.andypj.xyz/gtxhjhghdk.html

[U09] Py：字典取最大值的键
来源：http://hz.cdnleiting.top/gtgipxrpqa.html

max(d, key=d.get)
来源：http://hz.andypj.xyz/gtqovofgyp.html

[U10] Py：按值排序字典
来源：http://hz.xingfuxueyuan.xyz/gtrbwtwbue.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.meibo888.top/gtolhqotgx.html

[U11] Py：生成器表达式
来源：http://hz.smart0.xyz/gtxypnyegw.html

(x * 2 for x in arr)
来源：http://hz.svipenyu.cn/gttjunzaqd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xinyue.icu/gtxjuzkfcy.html

Counter(arr).most_common(3)
来源：http://hz.quarkkingdee.top/gtswzlwtpj.html

[U13] Py：固定长度队列
来源：http://hz.birdmap.top/gtvthomclp.html

deque(maxlen=10)
来源：http://hz.svipenyu.cn/gtaawfremi.html

[U14] Py：分组收集到列表
来源：http://hz.snrcjt.cn/gtcqycfftz.html

defaultdict(list)
来源：http://hz.zhengqikj.top/gtqdqvawmu.html

[U15] Py：高精度计时
来源：http://hz.cashguo.top/gtaoxuvryy.html

t = time.perf_counter()
来源：http://hz.yuxming.cn/gtguglhkvn.html

[U16] Py：命令行参数解析
来源：http://hz.wangdashe.top/gtspnebjcv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.fzhhl.top/gtaqyfcnxd.html

[U17] Py：初始化日志
来源：http://hz.daxiang520.top/gtebwzkjdw.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.redwolf501.top/gtjuqnbdqu.html

[U18] Py：预编译正则
来源：http://hz.yvedp.cn/gtmljlpisx.html

pat = re.compile(r"\d+")
来源：http://hz.cdnleiting.top/gteorpwmfh.html

[U19] Py：正则替换带回调
来源：http://hz.yj20258888.top/gtndphbeid.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shzxlz.cn/gtkkadgugl.html

[U20] Py：缓存函数结果
来源：http://hz.zhixingplan.top/gtvfwrvqat.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhaomingkeji.xyz/gtgvholkmi.html

[U21] Py：自定义上下文管理器
来源：http://hz.guowangkeji.top/gtripuiirr.html

@contextlib.contextmanager
来源：http://hz.zhongyouzk.top/gtivdbqbuj.html

[U22] Py：矩阵转置
来源：http://hz.ehwqpu.com/gtaxxvvkoa.html

list(zip(*m))
来源：http://hz.gogol.net.cn/gtkolulagi.html

[U23] Py：分块读取大文件
来源：http://hz.ppjwa.cn/gtpqqwjejv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.wangdashe.top/gtwnwfkdtk.html

[U24] Py：路径操作
来源：http://hz.redwolf501.top/gtsxfrlbrr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zdqjudy.top/gtbekaymcm.html

[U25] Py：CSV 按字典读
来源：http://hz.zhengqikj.top/gtvkanwrgy.html

csv.DictReader(f)
来源：http://hz.iojbl.cn/gtlagjdosq.html

[U26] Py：并发下载
来源：http://hz.quarkkingdee.top/gtuufrkyll.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jiagoushi.top/gtieshjypa.html

[U27] Py：异步 HTTP
来源：http://hz.jlsjyb.cn/gtihlcsnsa.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jqgufenzy.top/gtzyjghvhz.html

[U28] Py：类型别名
来源：http://hz.havefunace.top/gtroeyzprl.html

UserId = int
来源：http://hz.jianghu66.top/gtsoqouocd.html

[U29] Py：属性校验
来源：http://hz.quarkkingdee.top/gtgnwyrkhq.html

@property 与 @x.setter 配合
来源：http://hz.shanyushiyangkeji.top/gtikavhuou.html

[U30] Py：数据类
来源：http://hz.xinyue.icu/gtxlnudxok.html

@dataclass(slots=True)
来源：http://hz.daria6918.cn/gtacjgmthy.html

[U31] Py：单测
来源：http://hz.kuanghao11.cn/gtqbgextoo.html

python -m pytest -q
来源：http://hz.hfpthk.cn/gtvidqudjx.html

[U32] Py：代码格式化
来源：http://hz.jinqigfzy.top/gtovazrgqa.html

ruff format . && ruff check --fix .
来源：http://hz.zhiwuduotai.top/gtwhtvcldp.html

[U33] Py：打包发布
来源：http://hz.xuetiantiany.cn/gtaueevqex.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jianghu66.top/gtiwsibril.html

[U34] Py：判断编码
来源：http://hz.gogol.net.cn/gtqofhnuom.html

chardet.detect(raw)
来源：http://hz.xingfuxueyuan.xyz/gtyafnbugr.html

[U35] Py：发送邮件
来源：http://hz.shzxlz.cn/gtmmgkowst.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.snrcjt.cn/gtumrfzdlc.html

[U36] Py：定时任务
来源：http://hz.ybcxt.top/gtfpsyyvnv.html

schedule.every(10).minutes.do(job)
来源：http://hz.jiagoushi.top/gtecjxxmkb.html

[U37] Py：读写 Excel
来源：http://hz.quarkkingdee.top/gtzlpcfpdi.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.dashuyun.cn/gtdkaaxuhp.html

[U38] Py：获取脚本所在目录
来源：http://hz.mhx1999.top/gtlhctwayb.html

Path(__file__).resolve().parent
来源：http://hz.yonumen.top/gtaybrekym.html

[U39] Py：判断是否在交互环境
来源：http://hz.cdnleiting.top/gtlhluhnxw.html

sys.stdout.isatty()
来源：http://hz.haohaochexian.top/gtinesvuro.html

[U40] Py：打印到标准错误
来源：http://hz.gzhubu.top/gtgrhparyg.html

print("err", file=sys.stderr)
来源：http://hz.zdqjudy.top/gtpojpwzyk.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.0kj1m.cn/gtjkgiyjtm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhixingplan.top/gtengkrsqq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shangyingyoupin.top/gtcdczlojt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.c1oappe.top/gtsjfgbvxb.html

[U43] PHP：声明命名空间
来源：http://hz.sufxvd.cn/gtzdmnqhhw.html

namespace App\Http;
来源：http://hz.yuxming.cn/gtlkweobpj.html

[U44] PHP：开启严格类型
来源：http://hz.jinqigfzy.top/gtljpnzsfa.html

declare(strict_types=1);
来源：http://hz.hongshengwenyu.top/gtgbctwqqa.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jyoumei.cn/gtcvhgmqtt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangkeji.top/gtpclgerbq.html

[U46] PHP：可空类型
来源：http://hz.jlsjyb.cn/gtoabefrgx.html

?string $name = null
来源：http://hz.fengsongda.top/gtbqlkcdwh.html

[U47] PHP：联合类型
来源：http://hz.ppjwa.cn/gtgzhdktra.html

int|string $id
来源：http://hz.aizwys.cn/gtmakwsoza.html

[U48] PHP：纯枚举
来源：http://hz.birdmap.top/gtxrrncxkb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.dashuyun.cn/gtlnxhfnqb.html


<!-- 参考信息 -->