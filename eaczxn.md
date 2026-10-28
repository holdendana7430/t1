代发 wailian999

static int counter = 0;
来源：http://hz.redwolf501.top/gtqtkbsvmx.html

[S29] C：变参函数
来源：http://hz.cdnleiting.top/gtqgaervjb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yuxming.cn/gtvolqvyte.html

[S30] C：头文件保护
来源：http://hz.gzhubu.top/gtvdwwruoc.html

#ifndef X_H
来源：http://hz.gaohongyu789.top/gtkekdqgzq.html

#define X_H
来源：http://hz.yuanzhike.top/gtzlifadau.html

#endif
来源：http://hz.yongpay.top/gtiiquqemy.html

[S31] C++：Hello World
来源：http://hz.xziqi.cn/gtjulzveza.html

#include <iostream>
来源：http://hz.bjfxy.top/gtstybwqri.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigfzy.top/gthcppsrac.html

[S32] C++：字符串
来源：http://hz.jqgufenzy.top/gtrkbolvja.html

std::string s = "hi";  s += "!";
来源：http://hz.zhijiandao.cn/gtvkqkansv.html

[S33] C++：vector 增删
来源：http://hz.guowangkeji.top/gtuuazqxrf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgufenzy.top/gtlmqhxnzg.html

[S34] C++：遍历 vector
来源：http://hz.svipenyu.cn/gtibdyzvrh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gogol.net.cn/gtiqovsmwr.html

[S35] C++：map
来源：http://hz.sweek.top/gtfavhdghb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtctoedojw.html

[S36] C++：unordered_map
来源：http://hz.yuxming.cn/gtgyfbgenj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydjk.org.cn/gtseqgyiat.html

[S37] C++：set
来源：http://hz.zhongyouzk.top/gtpbybiivy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aizwys.cn/gtmftguiwn.html

[S38] C++：排序
来源：http://hz.cqqwz.cn/gtageilnbe.html

std::sort(v.begin(), v.end());
来源：http://hz.yuanzhike.top/gtmrrryyqw.html

[S39] C++：自定义比较器排序
来源：http://hz.cdnleiting.top/gtgwkcjzeg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tian-w.cn/gtkycrlkjm.html

[S40] C++：查找元素
来源：http://hz.hnxiangtu.top/gtlsztuolm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gogol.net.cn/gtaffuwdww.html

[S41] C++：类与构造函数
来源：http://hz.ivvv.top/gttzwfpjwf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinyuanbaomall.cn/gtradtlnvn.html

[S42] C++：继承与虚函数
来源：http://hz.yongpay.top/gtwtlxgdgw.html

class B : public Base { public: void f() override {} };
来源：http://hz.daria6918.cn/gtzryinfrd.html

[S43] C++：智能指针
来源：http://hz.yangfankeji.com/gtphrvbiol.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenlongwang.top/gtlsnwsddg.html

[S44] C++：引用传参
来源：http://hz.smart0.xyz/gtqznugyot.html

void inc(int &x) { ++x; }
来源：http://hz.xylfe.cn/gtgsizbcbb.html

[S45] C++：lambda
来源：http://hz.guannengcc.top/gtacnnvrzm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aibaodan.cn/gtfxrmefzd.html

[S46] C++：函数模板
来源：http://hz.kuanghao11.cn/gtknkfetyi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhengqikj.top/gtofggjzzt.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhijiandao.cn/gtcumqsdks.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yanxiufei.cn/gtctsmgihh.html

[S48] C++：逐行读文件
来源：http://hz.xingfuxueyuan.xyz/gteupfyjmq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hysaishi.cn/gtghrnauvb.html

while (std::getline(in, line)) { }
来源：http://hz.zhaomingkeji.xyz/gtivywregi.html

[S49] C++：写文件
来源：http://hz.jinqigufen.top/gttscdzesw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj202588.top/gtdavbfwdg.html

[S50] C++：格式化数字
来源：http://hz.yvedp.cn/gtzuyoyneo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gaohongyu789.top/gtaxsskhrs.html

[S51] C++：显式类型转换
来源：http://hz.chenlongwang.top/gtndejbwpc.html

static_cast<double>(a) / b
来源：http://hz.haohaochexian.top/gtotlulhtl.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258.top/gtnbvwroni.html

int size() const noexcept { return n_; }
来源：http://hz.mhx1999.top/gtlwvdrjmj.html

[S53] C++：移动语义
来源：http://hz.xziqi.cn/gtcjbciueq.html

std::vector<int> w = std::move(v);
来源：http://hz.fengsongda.top/gtgjaekmmu.html

[S54] C++：异常处理
来源：http://hz.sysykeji.top/gtdwjoeroa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hfpthk.cn/gtrelsfcam.html

[S55] C++：结构化绑定
来源：http://hz.chenjidiqi.icu/gtfusgkkam.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhoulong.xyz/gtejpzocdr.html

[S56] C++：optional
来源：http://hz.zhijiandao.cn/gtatqrjgwp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xylfe.cn/gtfryydeck.html

[S57] C++：编译期常量
来源：http://hz.jinqigufen.top/gtxxalivzm.html

constexpr int N = 10;
来源：http://hz.yuanzhike.top/gtqfmpzrai.html

[S58] C++：命名空间
来源：http://hz.yangfankeji.com/gtckebmenx.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxinkj.top/gtvxasrxny.html

[S59] C++：静态断言
来源：http://hz.xingfuxueyuan.xyz/gtrzegivix.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.mhx1999.top/gtwbqvdkfc.html

[S60] C++：遍历并删除元素
来源：http://hz.zdqjudy.top/gtyrqvpuat.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shangyingyoupin.top/gtjicmwilh.html

================================================================================
来源：http://hz.smart0.xyz/gtrulgnndy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sufxvd.cn/gtkfutdubu.html

================================================================================
来源：http://hz.haohaochexian.top/gtslaxjszw.html

[T01] Kotlin：Hello World
来源：http://hz.gaohongyu789.top/gtotcsoevc.html

println("Hello")
来源：http://hz.yj20258888.top/gtpstkkebr.html

[T02] Kotlin：变量
来源：http://hz.yonumen.top/gtnlvjcyms.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hongshengwenyu.top/gtixzrywbk.html

[T03] Kotlin：字符串模板
来源：http://hz.iojbl.cn/gtmenmdrjj.html

"值: $b"
来源：http://hz.hysaishi.cn/gtucphmvba.html

[T04] Kotlin：空安全
来源：http://hz.jinyuanbaomall.cn/gtcyvlnulk.html

val n: String? = null;  n?.length
来源：http://hz.tianlin.xyz/gtzwzkyend.html

[T05] Kotlin：when 表达式
来源：http://hz.zycfv.cn/gtgbqdqlwg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tianlin.xyz/gtubnnynmf.html

[T06] Kotlin：集合映射
来源：http://hz.xziqi.cn/gtwlcjjgxb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhongyouzk.top/gtbavaekwc.html

[T07] Kotlin：集合过滤
来源：http://hz.wangshuangyany.cn/gtxtuerkcs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nwbrower.top/gtpzcpewyi.html

[T08] Kotlin：数据类
来源：http://hz.jqgfzy.top/gtttttrbkk.html

data class User(val name: String, val age: Int)
来源：http://hz.dashuyun.cn/gtdiruickz.html

[T09] Kotlin：扩展函数
来源：http://hz.tanke756.top/gtqgoaojug.html

fun String.exclaim() = this + "!"
来源：http://hz.hfpthk.cn/gtuubnegij.html

[T10] Kotlin：默认参数
来源：http://hz.pengpengdd.cyou/gtdkbrdvut.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aibaodan.cn/gtslsmcxuc.html

[T11] Kotlin：协程
来源：http://hz.jinqigufen.top/gtmriyzpoj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenzaomai.com/gttgmszmyt.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtirtixbks.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj20258888.top/gtzakahyjy.html

[T13] Kotlin：只读 Map
来源：http://hz.hnxiangtu.top/gtbliubxmn.html

val m = mapOf("a" to 1)
来源：http://hz.vqdsnc.cn/gtzieqlmzv.html

[T14] Kotlin：循环
来源：http://hz.quarkkingdee.top/gtcxknlpcn.html

for (i in 1..10) println(i)
来源：http://hz.hfpthk.cn/gtdbntbulw.html

[T15] Kotlin：接口
来源：http://hz.sxryk.cn/gtybjbkvln.html

interface Shape { fun area(): Double }
来源：http://hz.xinyue.icu/gttvtuwzfw.html

[T16] Swift：Hello World
来源：http://hz.hongshengwenyu.top/gtiajrohay.html

print("Hello")
来源：http://hz.sysykeji.top/gtrqhnxwzl.html

[T17] Swift：变量与常量
来源：http://hz.316326.xyz/gtmzjpziji.html

var a = 1;  let b = 2
来源：http://hz.xuanzx.com/gthufdayaz.html

[T18] Swift：字符串插值
来源：http://hz.sufxvd.cn/gtqbnpgibb.html

"值: \(b)"
来源：http://hz.ybcxt.top/gthdtdvhdz.html

[T19] Swift：可选绑定
来源：http://hz.iojbl.cn/gtmgoszhiu.html

if let n = opt { print(n) }
来源：http://hz.jyoumei.cn/gtqzcmkino.html

[T20] Swift：数组操作
来源：http://hz.wangshuangyany.cn/gtyjbkxtly.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.316326.xyz/gtisumuafj.html

[T21] Swift：遍历
来源：http://hz.tian-w.cn/gtmurcqzpg.html

for x in a { print(x) }
来源：http://hz.yonumen.top/gtoguxwawd.html

[T22] Swift：字典
来源：http://hz.aizwys.cn/gttngyfrfr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.guannengcc.top/gtibblbjfs.html

[T23] Swift：函数
来源：http://hz.jinqigufen.top/gtzxivkrjd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.fzhhl.top/gtvqutqptn.html

[T24] Swift：闭包
来源：http://hz.gotoacloud.top/gtyyghpixh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj20258.top/gtejjdlapo.html

[T25] Swift：结构体
来源：http://hz.xylfe.cn/gtmkakrgmf.html

struct P { var x: Int }
来源：http://hz.andypj.xyz/gtjypsswsc.html

[T26] Swift：类与重写
来源：http://hz.zhongyouzk.top/gtdjpsrdpg.html

class A: Base { override func f() {} }
来源：http://hz.jiagoushi.top/gtcvkgswny.html

[T27] Swift：错误处理
来源：http://hz.wangdashe.top/gtmzzygyor.html

do { try f() } catch { print(error) }
来源：http://hz.cheryme.top/gtepctxwqd.html

[T28] Swift：枚举
来源：http://hz.fengsongda.top/gtyghemcvd.html

enum Color { case red, green }
来源：http://hz.yvedp.cn/gtrzcfxsun.html

[T29] Swift：guard 提前返回
来源：http://hz.birdmap.top/gtgksdnish.html

guard let x = opt else { return }
来源：http://hz.ydzc1.top/gtixjglzbm.html

[T30] Swift：协议
来源：http://hz.jinqigfzy.top/gtxddntpen.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigufen.top/gtreokiucx.html

[T31] Lua：Hello World
来源：http://hz.iojbl.cn/gtjjbfpjzn.html

print("Hello")
来源：http://hz.cucudq.cn/gtzqgzfpaq.html

[T32] Lua：局部变量
来源：http://hz.gzhubu.top/gtiuoxhlht.html

local a = 1
来源：http://hz.sweek.top/gtxrkjirxd.html

[T33] Lua：表（数组）
来源：http://hz.meibo888.top/gtlrokvpyl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.pengpengdd.cyou/gthkbfpwqn.html

[T34] Lua：遍历表
来源：http://hz.ywan-chungtsiang.top/gthciiwnhs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shzxlz.cn/gtsnschvtm.html

[T35] Lua：字典表
来源：http://hz.zhengqikj.top/gtogyhnhzr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ywan-chungtsiang.top/gtramcsjox.html

[T36] Lua：函数
来源：http://hz.ivvv.top/gtyxtzowbc.html

function add(a, b) return a + b end
来源：http://hz.mhx1999.top/gtygvziabf.html

[T37] Lua：字符串拼接
来源：http://hz.sysykeji.top/gtpighpqti.html

"a" .. "b"
来源：http://hz.iojbl.cn/gtyfkdkggd.html

[T38] Lua：条件
来源：http://hz.xingfuxueyuan.xyz/gtlgwnlfhv.html

if x > 0 then print("正") end
来源：http://hz.shanyushiyangtech.top/gtxmlcjeco.html

[T39] Lua：模式匹配
来源：http://hz.ydjk.org.cn/gtsrpbsdcw.html

string.find(s, "%d+")
来源：http://hz.birdmap.top/gttgeimzeb.html

[T40] Lua：元表
来源：http://hz.xingfuxueyuan.xyz/gtemitbxgs.html

setmetatable({}, { __index = base })
来源：http://hz.wangdashe.top/gtfpmugjtk.html

[T41] Perl：Hello World
来源：http://hz.jiagoushi.top/gtysfznxsz.html

print "Hello\n";
来源：http://hz.zhongyouzk.top/gtlgfsqbkh.html

[T42] Perl：变量类型
来源：http://hz.gaohongyu789.top/gteyywspvf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sufxvd.cn/gtppweodfy.html

[T43] Perl：字符串插值
来源：http://hz.xziqi.cn/gtjxlfpgnx.html

"值: $a"
来源：http://hz.fzhhl.top/gtudsoljui.html

[T44] Perl：条件
来源：http://hz.meibo888.top/gtbgmvfrzo.html

if ($a > 0) { print "正"; }
来源：http://hz.sweek.top/gtugsdwnbp.html

[T45] Perl：数组遍历
来源：http://hz.gaohongyu789.top/gtaqjentxh.html

for my $x (@arr) { print $x; }
来源：http://hz.hnqzz.top/gtnjvrvxfj.html

[T46] Perl：哈希操作
来源：http://hz.jqgufenzy.top/gtikuineis.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ydjk.org.cn/gtzwvmtkon.html

[T47] Perl：正则捕获
来源：http://hz.kuanghao11.cn/gtviakextp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yanxiufei.cn/gtbdtbcghk.html

[T48] Perl：正则替换
来源：http://hz.yuxming.cn/gtegeryovs.html

$s =~ s/old/new/g;
来源：http://hz.jqgufenzy.top/gtkaupllne.html

[T49] Perl：函数
来源：http://hz.guannengcc.top/gtsslsgjmh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zycfv.cn/gteadvrryb.html

[T50] Perl：逐行读文件
来源：http://hz.wangshuangyany.cn/gteexjsxyu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigufen.top/gtdhecsiwk.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xuanzx.com/gteasxrfhw.html

[T51] Scala：Hello World
来源：http://hz.yj20258.top/gtbcccisjg.html

println("Hello")
来源：http://hz.aibaodan.cn/gtwazkndke.html

[T52] Scala：变量
来源：http://hz.tianlin.xyz/gtusuetozr.html

val a = 1;  var b = 2
来源：http://hz.aibaodan.cn/gtcprjsqvm.html

[T53] Scala：字符串插值
来源：http://hz.gaohongyu789.top/gtnszdhqkk.html

s"值: $b"
来源：http://hz.feifeiyinyue.top/gtnvhmbryx.html

[T54] Scala：集合映射
来源：http://hz.hysaishi.cn/gtpshyetxj.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ydjk.org.cn/gtsvcvzgug.html

[T55] Scala：集合过滤
来源：http://hz.hysaishi.cn/gtcuospnic.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hysaishi.cn/gtjsbvfbfh.html

[T56] Scala：样例类
来源：http://hz.hywenlv.cn/gtnbotcubq.html

case class User(name: String, age: Int)
来源：http://hz.nanxuanxn.top/gtsdwrzpjy.html

[T57] Scala：模式匹配
来源：http://hz.zhijiandao.cn/gtfgneucjg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gotoacloud.top/gthkpqqtmm.html

[T58] Scala：函数定义
来源：http://hz.zycfv.cn/gtyicnqjzx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.fengsongda.top/gtewdfjbcx.html

[T59] Scala：循环
来源：http://hz.jqgfzy.top/gtelabngww.html

for (i <- 1 to 10) println(i)
来源：http://hz.zdqjudy.top/gtcubmkcwu.html

[T60] Scala：折叠
来源：http://hz.shangyingyoupin.top/gtnqvuiebn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.wangdashe.top/gtzqwdcggy.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtrgxtvgjz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tanke756.top/gthvinyxqe.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtkqyiptkz.html

[U01] Py：创建虚拟环境
来源：http://hz.0kj1m.cn/gttfuslwyp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yvedp.cn/gthuapmykd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhaomingkeji.xyz/gtrtpzyylv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhongyouzk.top/gtzfhsqwge.html

[U03] Py：加载 .env 配置
来源：http://hz.andypj.xyz/gtjbtciwyh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.c1oappe.top/gtjdxsbqjd.html

[U04] Py：变量调试打印
来源：http://hz.birdmap.top/gtotsdluta.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jiagoushi.top/gtyyohlfxu.html

[U05] Py：列表去重且保序
来源：http://hz.jinqigfzy.top/gtdrifrsai.html

list(dict.fromkeys(arr))
来源：http://hz.pycfn.com/gtmqxmunpp.html

[U06] Py：合并两个字典
来源：http://hz.nwbrower.top/gtxselibjw.html

{**a, **b}
来源：http://hz.yonumen.top/gtujupejup.html

[U07] Py：反转字典键值
来源：http://hz.dianchejie.cn/gtnmcbzsyv.html

{v: k for k, v in d.items()}
来源：http://hz.sysykeji.top/gtzaqykyag.html

[U08] Py：展平二维列表
来源：http://hz.sweek.top/gthzyabrme.html

[y for x in nested for y in x]
来源：http://hz.nanxinkj.top/gtbscvojec.html

[U09] Py：字典取最大值的键
来源：http://hz.ehwqpu.com/gtynldbkdw.html

max(d, key=d.get)
来源：http://hz.shuidangran.top/gtukzmhnse.html

[U10] Py：按值排序字典
来源：http://hz.pycfn.com/gtjxtblkky.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cucudq.cn/gtilzovfai.html

[U11] Py：生成器表达式
来源：http://hz.hnxiangtu.top/gtxzbremml.html

(x * 2 for x in arr)
来源：http://hz.ydzc1.top/gtgxcgnjck.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.aizwys.cn/gthmfcnrdj.html

Counter(arr).most_common(3)
来源：http://hz.sufxvd.cn/gtenrzwqlu.html

[U13] Py：固定长度队列
来源：http://hz.dashuyun.cn/gtkihdxufs.html

deque(maxlen=10)
来源：http://hz.jlsjyb.cn/gtllibkhaw.html

[U14] Py：分组收集到列表
来源：http://hz.snrcjt.cn/gtxgipthwy.html

defaultdict(list)
来源：http://hz.xuetiantiany.cn/gttiffyeqg.html

[U15] Py：高精度计时
来源：http://hz.andypj.xyz/gtgihummji.html

t = time.perf_counter()
来源：http://hz.ywan-chungtsiang.top/gtvosqcucr.html

[U16] Py：命令行参数解析
来源：http://hz.fengsongda.top/gtpftrepih.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xylfe.cn/gtlzvurppx.html

[U17] Py：初始化日志
来源：http://hz.jinqigfzy.top/gtaagzwuoi.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.nanxuanxn.top/gtlkwmdqqc.html

[U18] Py：预编译正则
来源：http://hz.316326.xyz/gtvgbylnlc.html

pat = re.compile(r"\d+")
来源：http://hz.chenzaomai.com/gtejstvbrp.html

[U19] Py：正则替换带回调
来源：http://hz.havefunace.top/gtvbagqjom.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhijiandao.cn/gtljlkjjld.html

[U20] Py：缓存函数结果
来源：http://hz.havefunace.top/gttwmhwurg.html

@functools.lru_cache(maxsize=None)
来源：http://hz.mhx1999.top/gtwyjhbdfb.html

[U21] Py：自定义上下文管理器
来源：http://hz.daria6918.cn/gteqmnkijc.html

@contextlib.contextmanager
来源：http://hz.jiagoushi.top/gtfitbctsh.html

[U22] Py：矩阵转置
来源：http://hz.fengsongda.top/gtglxfbfzk.html

list(zip(*m))
来源：http://hz.mhx1999.top/gtmnjlkuaa.html

[U23] Py：分块读取大文件
来源：http://hz.meibo888.top/gtaqlsgqnt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.nwbrower.top/gtgxljqswm.html

[U24] Py：路径操作
来源：http://hz.zhixingplan.top/gtkxwczsfm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yj202588.top/gtkwkhhopg.html

[U25] Py：CSV 按字典读
来源：http://hz.ywan-chungtsiang.top/gtqjmdinda.html

csv.DictReader(f)
来源：http://hz.ybcxt.top/gtdgchpilj.html

[U26] Py：并发下载
来源：http://hz.meibo888.top/gtxvodrcsh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jianghu66.top/gtptocutwb.html

[U27] Py：异步 HTTP
来源：http://hz.fengsongda.top/gtfqsejqan.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ydzc1.top/gtqysasbmi.html

[U28] Py：类型别名
来源：http://hz.zhijiandao.cn/gtttlwprrp.html

UserId = int
来源：http://hz.yuxming.cn/gtuyajudvt.html

[U29] Py：属性校验
来源：http://hz.yj20258888.top/gthentzxjm.html

@property 与 @x.setter 配合
来源：http://hz.guannengcc.top/gtiaewycpk.html

[U30] Py：数据类
来源：http://hz.gaohongyu789.top/gtglihqyyx.html

@dataclass(slots=True)
来源：http://hz.yueranfly.top/gthbsugqgj.html

[U31] Py：单测
来源：http://hz.bjfxy.top/gtzuypyuoa.html

python -m pytest -q
来源：http://hz.yueranfly.top/gtkiuzilzl.html

[U32] Py：代码格式化
来源：http://hz.dashuyun.cn/gtkhgwaeeu.html

ruff format . && ruff check --fix .
来源：http://hz.haohaochexian.top/gtowxxnfpn.html

[U33] Py：打包发布
来源：http://hz.0kj1m.cn/gtifmbvnho.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.aizwys.cn/gtajjkdxjf.html

[U34] Py：判断编码
来源：http://hz.zdqjudy.top/gthwynfovh.html

chardet.detect(raw)
来源：http://hz.yuxming.cn/gtbxgqfnxk.html

[U35] Py：发送邮件
来源：http://hz.jiagoushi.top/gtlbbugnkd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.wangdashe.top/gtopugdchq.html

[U36] Py：定时任务
来源：http://hz.ivvv.top/gtyrqxtmsh.html

schedule.every(10).minutes.do(job)
来源：http://hz.xinyue.icu/gtfmejrfyf.html

[U37] Py：读写 Excel
来源：http://hz.ppjwa.cn/gtupquilbq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.feifeiyinyue.top/gtsqsjigiq.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhiwuduotai.top/gthqzoqpvu.html

Path(__file__).resolve().parent
来源：http://hz.daria6918.cn/gtmtgpyscq.html

[U39] Py：判断是否在交互环境
来源：http://hz.ydjk.org.cn/gtlemezsxw.html

sys.stdout.isatty()
来源：http://hz.iojbl.cn/gttlaztbxv.html

[U40] Py：打印到标准错误
来源：http://hz.52xcode.cn/gthaknoonp.html

print("err", file=sys.stderr)
来源：http://hz.yj20258.top/gtgeeuohff.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.aibaodan.cn/gtcqoigmif.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.mhx1999.top/gtpbwgehsx.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.meibo888.top/gtkmvpyfrt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhongyouzk.top/gtfekwvvol.html

[U43] PHP：声明命名空间
来源：http://hz.kuanghao11.cn/gtcchtbwpv.html

namespace App\Http;
来源：http://hz.52xcode.cn/gthrgrerkp.html

[U44] PHP：开启严格类型
来源：http://hz.sufxvd.cn/gtunbuayfd.html

declare(strict_types=1);
来源：http://hz.jqgfzy.top/gtrwvumhww.html

[U45] PHP：类型声明与返回类型
来源：http://hz.pycfn.com/gtwlwoktlm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gtbxjskclv.html

[U46] PHP：可空类型
来源：http://hz.dianchejie.cn/gtboogmyah.html

?string $name = null
来源：http://hz.xuanzx.com/gtrlwqromv.html

[U47] PHP：联合类型
来源：http://hz.gogol.net.cn/gtbnbmrpyf.html

int|string $id
来源：http://hz.jyoumei.cn/gtexifwhdg.html

[U48] PHP：纯枚举
来源：http://hz.guowangkeji.top/gtnlmjqtry.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xuetiantiany.cn/gtsxukxhdp.html

[U49] PHP：只读属性
来源：http://hz.ehwqpu.com/gtkrubvamy.html

public readonly string $name
来源：http://hz.pycfn.com/gtvslaqtpd.html

[U50] PHP：构造器属性提升
来源：http://hz.dashuyun.cn/gtdwdfhebc.html

public function __construct(private int $id) {}
来源：http://hz.yj202588.top/gtowtyhstj.html

[U51] PHP：数组解构
来源：http://hz.jyoumei.cn/gtfgjuhijs.html

[$a, $b] = $arr;
来源：http://hz.hnqzz.top/gtvrrlabbi.html

[U52] PHP：箭头函数
来源：http://hz.shanyushiyangtech.top/gtrsdjguvw.html

$double = fn($x) => $x * 2;
来源：http://hz.tianlin.xyz/gtwjwskmul.html


<!-- 参考信息 -->