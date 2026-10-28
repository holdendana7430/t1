代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fengsongda.top/gtufpelwsr.html

[S23] C：随机数
来源：http://hz.yj20258888.top/gtftljhgom.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.316326.xyz/gtbrzyyhbp.html

[S24] C：获取本地时间
来源：http://hz.yj20258888.top/gtpnbwtiux.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.haohaochexian.top/gtwdifyapt.html

[S25] C：内存拷贝
来源：http://hz.wangdashe.top/gtocnhwkdx.html

memcpy(dst, src, n);
来源：http://hz.meibo888.top/gtytrqstsx.html

[S26] C：内存清零
来源：http://hz.9152youxi.cn/gtaeqfocmm.html

memset(a, 0, sizeof a);
来源：http://hz.dashuyun.cn/gtgwevkjov.html

[S27] C：定义常量
来源：http://hz.ivvv.top/gtjlzwtmmn.html

const double PI = 3.14159;
来源：http://hz.zdqjudy.top/gtrrlolcrf.html

[S28] C：静态变量
来源：http://hz.aibaodan.cn/gtmbtzaqso.html

static int counter = 0;
来源：http://hz.guowangkeji.top/gthkpopdby.html

[S29] C：变参函数
来源：http://hz.shanyushiyangkeji.top/gtxlwxrmsj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.wangdashe.top/gthkzrlwsr.html

[S30] C：头文件保护
来源：http://hz.feifeiyinyue.top/gttzonktxa.html

#ifndef X_H
来源：http://hz.wangdashe.top/gtvwucalch.html

#define X_H
来源：http://hz.yueranfly.top/gtpbvhoalq.html

#endif
来源：http://hz.jqgfzy.top/gttczskaqw.html

[S31] C++：Hello World
来源：http://hz.birdmap.top/gthuzucehf.html

#include <iostream>
来源：http://hz.xinyue.icu/gtsccncssk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yueranfly.top/gtlygkqswj.html

[S32] C++：字符串
来源：http://hz.iojbl.cn/gtspwabemh.html

std::string s = "hi";  s += "!";
来源：http://hz.meibo888.top/gtvtfowmvz.html

[S33] C++：vector 增删
来源：http://hz.shuidangran.top/gtajxswnzc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xingfuxueyuan.xyz/gtkzrqophq.html

[S34] C++：遍历 vector
来源：http://hz.hysaishi.cn/gtqopmlggq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hywenlv.cn/gtcgrmpjul.html

[S35] C++：map
来源：http://hz.zhiwuduotai.top/gtwxbfbtjp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hammf.cn/gtcsmbunrd.html

[S36] C++：unordered_map
来源：http://hz.zhixingplan.top/gtpxiwtqiz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hammf.cn/gtkfngbckc.html

[S37] C++：set
来源：http://hz.jinqigfzy.top/gtogoovlpm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gotoacloud.top/gtdiynbntw.html

[S38] C++：排序
来源：http://hz.birdmap.top/gtosngjvzb.html

std::sort(v.begin(), v.end());
来源：http://hz.chenlongwang.top/gtktpgljbd.html

[S39] C++：自定义比较器排序
来源：http://hz.snrcjt.cn/gtuuidzxvg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sxryk.cn/gtnosizoqs.html

[S40] C++：查找元素
来源：http://hz.cucudq.cn/gtjsyrtcqt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhiwuduotai.top/gtlncuixta.html

[S41] C++：类与构造函数
来源：http://hz.daria6918.cn/gtwfvgolis.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hywenlv.cn/gtwrfjvaxj.html

[S42] C++：继承与虚函数
来源：http://hz.tian-w.cn/gtdrdpzmjt.html

class B : public Base { public: void f() override {} };
来源：http://hz.fengsongda.top/gtophjpavg.html

[S43] C++：智能指针
来源：http://hz.bjfxy.top/gttfwvaqqc.html

auto p = std::make_unique<int>(5);
来源：http://hz.havefunace.top/gtqizjisqv.html

[S44] C++：引用传参
来源：http://hz.xingfuxueyuan.xyz/gttvkomzzj.html

void inc(int &x) { ++x; }
来源：http://hz.xingfuxueyuan.xyz/gtaowlnbuj.html

[S45] C++：lambda
来源：http://hz.fengsongda.top/gtrgrxlrav.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ydjk.org.cn/gtqczspulq.html

[S46] C++：函数模板
来源：http://hz.snrcjt.cn/gtbbvvtmna.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gzhubu.top/gtrmdgjhyt.html

[S47] C++：结构化绑定遍历
来源：http://hz.kuanghao11.cn/gtljscnhsl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jlsjyb.cn/gtzyrnlwtw.html

[S48] C++：逐行读文件
来源：http://hz.zhixingplan.top/gtueydqskx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhoulong.xyz/gtpvauocks.html

while (std::getline(in, line)) { }
来源：http://hz.cashguo.top/gtmttptwqu.html

[S49] C++：写文件
来源：http://hz.xziqi.cn/gtztgdpeba.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.iojbl.cn/gtkleuvavz.html

[S50] C++：格式化数字
来源：http://hz.gaohongyu789.top/gtqvwjqfub.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.quarkkingdee.top/gtumxaetqm.html

[S51] C++：显式类型转换
来源：http://hz.pycfn.com/gthguzzkot.html

static_cast<double>(a) / b
来源：http://hz.wangshuangyany.cn/gtxdjscocn.html

[S52] C++：const 与 noexcept
来源：http://hz.guannengcc.top/gtmpqilrrd.html

int size() const noexcept { return n_; }
来源：http://hz.nanxinkj.top/gtchlntobd.html

[S53] C++：移动语义
来源：http://hz.bjfxy.top/gtixorwbeb.html

std::vector<int> w = std::move(v);
来源：http://hz.yj202588.top/gtiqnitdim.html

[S54] C++：异常处理
来源：http://hz.tianlin.xyz/gtymmakvsg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.havefunace.top/gtyvkosvyp.html

[S55] C++：结构化绑定
来源：http://hz.sysykeji.top/gtgdzfwlxh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hnqzz.top/gtxynbtkhx.html

[S56] C++：optional
来源：http://hz.shzxlz.cn/gttguossba.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.svipenyu.cn/gtwukhubfb.html

[S57] C++：编译期常量
来源：http://hz.mhx1999.top/gtakueghgt.html

constexpr int N = 10;
来源：http://hz.jyoumei.cn/gtedbhdmns.html

[S58] C++：命名空间
来源：http://hz.jyoumei.cn/gtgpajvnum.html

namespace ns { int f() { return 1; } }
来源：http://hz.cashguo.top/gtzklbgrde.html

[S59] C++：静态断言
来源：http://hz.hnqzz.top/gtnuizvrnz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tianlin.xyz/gtxsnpdjsw.html

[S60] C++：遍历并删除元素
来源：http://hz.dianchejie.cn/gtpkyypsqh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinyuanbaomall.cn/gtvfytnqmf.html

================================================================================
来源：http://hz.dianchejie.cn/gtlfceebqv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.vqdsnc.cn/gtrflhjmcp.html

================================================================================
来源：http://hz.birdmap.top/gtxariliwl.html

[T01] Kotlin：Hello World
来源：http://hz.smart0.xyz/gtbssjbxdw.html

println("Hello")
来源：http://hz.yuanzhike.top/gtrlrmczho.html

[T02] Kotlin：变量
来源：http://hz.yanxiufei.cn/gtisnpcjmr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xingfuxueyuan.xyz/gttpjeshdv.html

[T03] Kotlin：字符串模板
来源：http://hz.xingfuxueyuan.xyz/gtskxisrnh.html

"值: $b"
来源：http://hz.gzhubu.top/gtpljuhxfg.html

[T04] Kotlin：空安全
来源：http://hz.shzxlz.cn/gtqgfrylti.html

val n: String? = null;  n?.length
来源：http://hz.zycfv.cn/gtgltrltrs.html

[T05] Kotlin：when 表达式
来源：http://hz.iojbl.cn/gtdmmfwish.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinghuilouyu.cn/gtkufppcsg.html

[T06] Kotlin：集合映射
来源：http://hz.ivvv.top/gtmqoctzbd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xinyue.icu/gtfuwazhop.html

[T07] Kotlin：集合过滤
来源：http://hz.yangfankeji.com/gtcxzndbcy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nanxinkj.top/gtixqujdat.html

[T08] Kotlin：数据类
来源：http://hz.shangyingyoupin.top/gtqaamyqyt.html

data class User(val name: String, val age: Int)
来源：http://hz.jyoumei.cn/gtmdjklgig.html

[T09] Kotlin：扩展函数
来源：http://hz.yuanzhike.top/gtjdygclkl.html

fun String.exclaim() = this + "!"
来源：http://hz.cashguo.top/gtvfmjbfzr.html

[T10] Kotlin：默认参数
来源：http://hz.sxryk.cn/gtixxhhnwi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ppjwa.cn/gtzbnnjrzp.html

[T11] Kotlin：协程
来源：http://hz.jiagoushi.top/gtrphtsgry.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shanyushiyangtech.top/gtksdavuem.html

[T12] Kotlin：解构声明
来源：http://hz.shangyingyoupin.top/gtdboiryyz.html

val (a, b) = Pair(1, 2)
来源：http://hz.jyoumei.cn/gtjmnvttix.html

[T13] Kotlin：只读 Map
来源：http://hz.pycfn.com/gtfplbgqwj.html

val m = mapOf("a" to 1)
来源：http://hz.cqqwz.cn/gtyrnxajtr.html

[T14] Kotlin：循环
来源：http://hz.daria6918.cn/gtwbsuasfd.html

for (i in 1..10) println(i)
来源：http://hz.havefunace.top/gtdfnseqhg.html

[T15] Kotlin：接口
来源：http://hz.ywan-chungtsiang.top/gtdtueqknf.html

interface Shape { fun area(): Double }
来源：http://hz.guannengcc.top/gtrsnfxvpr.html

[T16] Swift：Hello World
来源：http://hz.yanxiufei.cn/gtqnfqourx.html

print("Hello")
来源：http://hz.zhengqikj.top/gtlkywxfdz.html

[T17] Swift：变量与常量
来源：http://hz.aibaodan.cn/gtiwizzhzx.html

var a = 1;  let b = 2
来源：http://hz.yvedp.cn/gtnvbfrhvs.html

[T18] Swift：字符串插值
来源：http://hz.jlsjyb.cn/gtnrrwzvox.html

"值: \(b)"
来源：http://hz.guowangkeji.top/gtwgudqljn.html

[T19] Swift：可选绑定
来源：http://hz.chenlongwang.top/gtqpmcvzav.html

if let n = opt { print(n) }
来源：http://hz.zhaomingkeji.xyz/gttwtxcxoq.html

[T20] Swift：数组操作
来源：http://hz.jinqigufen.top/gtdyjxpfbh.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xinyue.icu/gtbuuiahqs.html

[T21] Swift：遍历
来源：http://hz.aibaodan.cn/gtxctirmtn.html

for x in a { print(x) }
来源：http://hz.zhengqikj.top/gtpzgjbrxw.html

[T22] Swift：字典
来源：http://hz.shanyushiyangtech.top/gticxpswtm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yvedp.cn/gtlceiysis.html

[T23] Swift：函数
来源：http://hz.ydzc1.top/gteppmaezy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nanxinkj.top/gtcrvjbxft.html

[T24] Swift：闭包
来源：http://hz.c1oappe.top/gtcsaikznf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ywan-chungtsiang.top/gtlcyocvnv.html

[T25] Swift：结构体
来源：http://hz.zhengqikj.top/gttcnveksh.html

struct P { var x: Int }
来源：http://hz.zhongyouzk.top/gtglpdwqtw.html

[T26] Swift：类与重写
来源：http://hz.yj20258888.top/gtjijpzoad.html

class A: Base { override func f() {} }
来源：http://hz.yongpay.top/gttdzdtjrx.html

[T27] Swift：错误处理
来源：http://hz.yj20258888.top/gtsupftjjg.html

do { try f() } catch { print(error) }
来源：http://hz.iojbl.cn/gtkgwarhtm.html

[T28] Swift：枚举
来源：http://hz.jianghu66.top/gtnfvvtucf.html

enum Color { case red, green }
来源：http://hz.daria6918.cn/gtjpfoukaa.html

[T29] Swift：guard 提前返回
来源：http://hz.chenlongwang.top/gtxdpshcou.html

guard let x = opt else { return }
来源：http://hz.cdnleiting.top/gtluxfauav.html

[T30] Swift：协议
来源：http://hz.feifeiyinyue.top/gtnziyodxn.html

protocol Shape { func area() -> Double }
来源：http://hz.yuxming.cn/gtvniepnlz.html

[T31] Lua：Hello World
来源：http://hz.aibaodan.cn/gtkmiqxagf.html

print("Hello")
来源：http://hz.nwbrower.top/gtslfwedok.html

[T32] Lua：局部变量
来源：http://hz.xylfe.cn/gtiqhptyvx.html

local a = 1
来源：http://hz.pengpengdd.cyou/gtsfsgnlzy.html

[T33] Lua：表（数组）
来源：http://hz.sweek.top/gtodizbacn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.fzhhl.top/gtqftcvimo.html

[T34] Lua：遍历表
来源：http://hz.yvedp.cn/gtrbxixyah.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hnxiangtu.top/gtuhbplunu.html

[T35] Lua：字典表
来源：http://hz.kuanghao11.cn/gtcahqjlsc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ivvv.top/gtupedhaof.html

[T36] Lua：函数
来源：http://hz.aizwys.cn/gtrgjgcozu.html

function add(a, b) return a + b end
来源：http://hz.316326.xyz/gtjezhdfnq.html

[T37] Lua：字符串拼接
来源：http://hz.9152youxi.cn/gtebyjbnaa.html

"a" .. "b"
来源：http://hz.haohaochexian.top/gtpzktgbxs.html

[T38] Lua：条件
来源：http://hz.wangdashe.top/gtomyavljd.html

if x > 0 then print("正") end
来源：http://hz.cheryme.top/gtluzoxbqy.html

[T39] Lua：模式匹配
来源：http://hz.jinghuilouyu.cn/gtpxkaebxv.html

string.find(s, "%d+")
来源：http://hz.tianlin.xyz/gtpftjnnht.html

[T40] Lua：元表
来源：http://hz.aizwys.cn/gtskhqwqhl.html

setmetatable({}, { __index = base })
来源：http://hz.jinghuilouyu.cn/gtsxirjgcn.html

[T41] Perl：Hello World
来源：http://hz.zycfv.cn/gtsrlekwaw.html

print "Hello\n";
来源：http://hz.chenzaomai.com/gtbitwbjus.html

[T42] Perl：变量类型
来源：http://hz.hywenlv.cn/gtweidpnfb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.meibo888.top/gtovlyulmh.html

[T43] Perl：字符串插值
来源：http://hz.xuanzx.com/gtaoqnwxfc.html

"值: $a"
来源：http://hz.jinyuanbaomall.cn/gtrvlzlfxo.html

[T44] Perl：条件
来源：http://hz.yj20258888.top/gtdioasrlr.html

if ($a > 0) { print "正"; }
来源：http://hz.birdmap.top/gtirzfgwug.html

[T45] Perl：数组遍历
来源：http://hz.jqgufenzy.top/gtgjqsivuy.html

for my $x (@arr) { print $x; }
来源：http://hz.yangfankeji.com/gtjjxyhecm.html

[T46] Perl：哈希操作
来源：http://hz.aibaodan.cn/gtjyqcanoh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.dianchejie.cn/gtnubqfvsx.html

[T47] Perl：正则捕获
来源：http://hz.smart0.xyz/gtuwkgulbf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yuxming.cn/gtjysiqdhl.html

[T48] Perl：正则替换
来源：http://hz.hongshengwenyu.top/gtgrpndbtk.html

$s =~ s/old/new/g;
来源：http://hz.xuanzx.com/gtevimcdwp.html

[T49] Perl：函数
来源：http://hz.daxiang520.top/gtfvlhmbkm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.c1oappe.top/gtdydmofda.html

[T50] Perl：逐行读文件
来源：http://hz.zhiwuduotai.top/gtpqejmqhd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ehwqpu.com/gtviftlang.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yanxiufei.cn/gtgjxbsqow.html

[T51] Scala：Hello World
来源：http://hz.gogol.net.cn/gtcylwwabw.html

println("Hello")
来源：http://hz.jiagoushi.top/gtylwnxigh.html

[T52] Scala：变量
来源：http://hz.yonumen.top/gtjfqzlngf.html

val a = 1;  var b = 2
来源：http://hz.quarkkingdee.top/gthiriettr.html

[T53] Scala：字符串插值
来源：http://hz.daria6918.cn/gtrddabhsk.html

s"值: $b"
来源：http://hz.cucudq.cn/gtekjtnsen.html

[T54] Scala：集合映射
来源：http://hz.guowangkeji.top/gtxtqvjgpo.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yj202588.top/gtgbooaaus.html

[T55] Scala：集合过滤
来源：http://hz.yongpay.top/gtpawgjyua.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gogol.net.cn/gtzlacvflp.html

[T56] Scala：样例类
来源：http://hz.ppjwa.cn/gtlndzxyjc.html

case class User(name: String, age: Int)
来源：http://hz.cqqwz.cn/gttnivfjxv.html

[T57] Scala：模式匹配
来源：http://hz.guowangkeji.top/gtashshrfs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xinyue.icu/gtyzpcddvw.html

[T58] Scala：函数定义
来源：http://hz.hfpthk.cn/gtnzwqsniy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.daria6918.cn/gttydpzjem.html

[T59] Scala：循环
来源：http://hz.pycfn.com/gtplcxqjsi.html

for (i <- 1 to 10) println(i)
来源：http://hz.andypj.xyz/gtteawhamq.html

[T60] Scala：折叠
来源：http://hz.xingfuxueyuan.xyz/gtviseqfhu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.wangshuangyany.cn/gtavoomjuc.html

================================================================================
来源：http://hz.yj20258.top/gtkluxlyzk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yonumen.top/gtokrjifbf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtkfulbcnp.html

[U01] Py：创建虚拟环境
来源：http://hz.xingfuxueyuan.xyz/gtanxwnhnd.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yonumen.top/gtlgcjshoi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fzhhl.top/gtianxzzvj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhengqikj.top/gtvirloavm.html

[U03] Py：加载 .env 配置
来源：http://hz.xuanzx.com/gttsmygege.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhongyouzk.top/gtbhuopuxx.html

[U04] Py：变量调试打印
来源：http://hz.hammf.cn/gtrrdpbdeh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sysykeji.top/gtawvowtsj.html

[U05] Py：列表去重且保序
来源：http://hz.guowangkeji.top/gtvxyvjxav.html

list(dict.fromkeys(arr))
来源：http://hz.aibaodan.cn/gttvrrfydc.html

[U06] Py：合并两个字典
来源：http://hz.ppjwa.cn/gturinjdvm.html

{**a, **b}
来源：http://hz.fengsongda.top/gteblcrrfj.html

[U07] Py：反转字典键值
来源：http://hz.andypj.xyz/gtvblnylhj.html

{v: k for k, v in d.items()}
来源：http://hz.52xcode.cn/gtdmmyvamm.html

[U08] Py：展平二维列表
来源：http://hz.sweek.top/gtozvudhft.html

[y for x in nested for y in x]
来源：http://hz.shzxlz.cn/gtahzbhwga.html

[U09] Py：字典取最大值的键
来源：http://hz.zhiwuduotai.top/gtrdgpktoq.html

max(d, key=d.get)
来源：http://hz.yj20258.top/gtqqmohboy.html

[U10] Py：按值排序字典
来源：http://hz.andypj.xyz/gtcfxvgbcp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jlsjyb.cn/gtvlkujgfo.html

[U11] Py：生成器表达式
来源：http://hz.c1oappe.top/gtowbtuhsv.html

(x * 2 for x in arr)
来源：http://hz.9152youxi.cn/gtszemovtk.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jlsjyb.cn/gtlnzxkbhv.html

Counter(arr).most_common(3)
来源：http://hz.yj202588.top/gtfybvmjqp.html

[U13] Py：固定长度队列
来源：http://hz.wangshuangyany.cn/gtfhlujzqk.html

deque(maxlen=10)
来源：http://hz.daxiang520.top/gtifrwbakg.html

[U14] Py：分组收集到列表
来源：http://hz.tian-w.cn/gtxtbqjueo.html

defaultdict(list)
来源：http://hz.yj20258.top/gtrfrcyicg.html

[U15] Py：高精度计时
来源：http://hz.fengsongda.top/gtykwiythc.html

t = time.perf_counter()
来源：http://hz.kuanghao11.cn/gtprjwnsyn.html

[U16] Py：命令行参数解析
来源：http://hz.guannengcc.top/gttsjtvjqv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gaohongyu789.top/gtorzupqse.html

[U17] Py：初始化日志
来源：http://hz.shanyushiyangtech.top/gtyfdyhfdy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.gzhubu.top/gtacbqmdon.html

[U18] Py：预编译正则
来源：http://hz.daxiang520.top/gtscchffqy.html

pat = re.compile(r"\d+")
来源：http://hz.shanyushiyangtech.top/gtraezdviq.html

[U19] Py：正则替换带回调
来源：http://hz.hfpthk.cn/gthjgtuloo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.smart0.xyz/gtxxcrlgms.html

[U20] Py：缓存函数结果
来源：http://hz.xuanzx.com/gtzzynavod.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhongyouzk.top/gtxxptcynh.html

[U21] Py：自定义上下文管理器
来源：http://hz.zycfv.cn/gtxkycdolt.html

@contextlib.contextmanager
来源：http://hz.xylfe.cn/gtirmlsbvs.html

[U22] Py：矩阵转置
来源：http://hz.0kj1m.cn/gtysmjmoav.html

list(zip(*m))
来源：http://hz.meibo888.top/gtyonubizw.html

[U23] Py：分块读取大文件
来源：http://hz.wangdashe.top/gtbsrglxdw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.mhx1999.top/gtbewbuzjg.html

[U24] Py：路径操作
来源：http://hz.yj20258888.top/gtbmtnsvqo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ydjk.org.cn/gtypkgehot.html

[U25] Py：CSV 按字典读
来源：http://hz.redwolf501.top/gtccrujhco.html

csv.DictReader(f)
来源：http://hz.feifeiyinyue.top/gtwtwkepkz.html

[U26] Py：并发下载
来源：http://hz.ydjk.org.cn/gttfbpozvz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cqqwz.cn/gttvogqkoo.html

[U27] Py：异步 HTTP
来源：http://hz.xziqi.cn/gtgnqxvyab.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jianghu66.top/gtitvhvkkr.html

[U28] Py：类型别名
来源：http://hz.zdqjudy.top/gtzkexbdij.html

UserId = int
来源：http://hz.nanxuanxn.top/gthxacgubc.html

[U29] Py：属性校验
来源：http://hz.iojbl.cn/gtqeswwgol.html

@property 与 @x.setter 配合
来源：http://hz.cdnleiting.top/gtwtqzmwnb.html

[U30] Py：数据类
来源：http://hz.yvedp.cn/gtaoprwbqu.html

@dataclass(slots=True)
来源：http://hz.hywenlv.cn/gtcgbyelrg.html

[U31] Py：单测
来源：http://hz.cashguo.top/gtoghwutjo.html

python -m pytest -q
来源：http://hz.pengpengdd.cyou/gtnhmalrgx.html

[U32] Py：代码格式化
来源：http://hz.meibo888.top/gtyrpzjwvg.html

ruff format . && ruff check --fix .
来源：http://hz.yuxming.cn/gtqmgxocll.html

[U33] Py：打包发布
来源：http://hz.shanyushiyangkeji.top/gtndzyfzey.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yuanzhike.top/gtmpmzdqud.html

[U34] Py：判断编码
来源：http://hz.redwolf501.top/gtvwcbtypk.html

chardet.detect(raw)
来源：http://hz.yj20258888.top/gtrpvdazca.html

[U35] Py：发送邮件
来源：http://hz.smart0.xyz/gthdzkecbg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jqgfzy.top/gthtoloeqc.html

[U36] Py：定时任务
来源：http://hz.fzhhl.top/gtvsvcvbfl.html

schedule.every(10).minutes.do(job)
来源：http://hz.pengpengdd.cyou/gtrxgrfdid.html

[U37] Py：读写 Excel
来源：http://hz.hnxiangtu.top/gtiarlgrjw.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.tianlin.xyz/gtzerzbeqm.html

[U38] Py：获取脚本所在目录
来源：http://hz.guowangkeji.top/gtabisivdt.html

Path(__file__).resolve().parent
来源：http://hz.hfpthk.cn/gtewfulvan.html

[U39] Py：判断是否在交互环境
来源：http://hz.fzhhl.top/gtfdavkdle.html

sys.stdout.isatty()
来源：http://hz.ppjwa.cn/gtuasvdfip.html

[U40] Py：打印到标准错误
来源：http://hz.hammf.cn/gtecnspixp.html

print("err", file=sys.stderr)
来源：http://hz.jyoumei.cn/gtpruvybrl.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhiwuduotai.top/gtbufxqxpi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shanyushiyangkeji.top/gtoiektwha.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.kuanghao11.cn/gtswwvltsz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.daxiang520.top/gtawgbvhky.html

[U43] PHP：声明命名空间
来源：http://hz.jqgfzy.top/gtdyvuawbp.html

namespace App\Http;
来源：http://hz.guannengcc.top/gtjyvpizwr.html

[U44] PHP：开启严格类型
来源：http://hz.zycfv.cn/gtouulyfos.html

declare(strict_types=1);
来源：http://hz.xinyue.icu/gtwxjpxzdq.html

[U45] PHP：类型声明与返回类型
来源：http://hz.dashuyun.cn/gtqlneuece.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtpltpfxll.html

[U46] PHP：可空类型
来源：http://hz.hongshengwenyu.top/gtewzuakzr.html

?string $name = null
来源：http://hz.shzxlz.cn/gttmfvnqwn.html


<!-- 参考信息 -->