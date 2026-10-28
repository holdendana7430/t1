代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jlsjyb.cn/gtqnsgrbjd.html

[S25] C：内存拷贝
来源：http://hz.chenjidiqi.icu/gtamrtbzow.html

memcpy(dst, src, n);
来源：http://hz.wangdashe.top/gtrccmlbkh.html

[S26] C：内存清零
来源：http://hz.mhx1999.top/gtwzufbrtd.html

memset(a, 0, sizeof a);
来源：http://hz.tanke756.top/gttldxgbgn.html

[S27] C：定义常量
来源：http://hz.hywenlv.cn/gtdbdwbsoe.html

const double PI = 3.14159;
来源：http://hz.ppjwa.cn/gtsewsjipg.html

[S28] C：静态变量
来源：http://hz.jinghuilouyu.cn/gtfbbnzahh.html

static int counter = 0;
来源：http://hz.jinqigufen.top/gtlnwivkog.html

[S29] C：变参函数
来源：http://hz.shanyushiyangkeji.top/gtjdsezpwj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.vqdsnc.cn/gtjqhpyzgy.html

[S30] C：头文件保护
来源：http://hz.haohaochexian.top/gtttlyciwv.html

#ifndef X_H
来源：http://hz.hywenlv.cn/gthoegqehw.html

#define X_H
来源：http://hz.dianchejie.cn/gtvdqjulpq.html

#endif
来源：http://hz.chenlongwang.top/gtnjvtvzyk.html

[S31] C++：Hello World
来源：http://hz.tanke756.top/gtqwoxdutz.html

#include <iostream>
来源：http://hz.zhijiandao.cn/gtuyjlcphh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.9152youxi.cn/gtbfwgcstj.html

[S32] C++：字符串
来源：http://hz.zhijiandao.cn/gtbzxyrqvj.html

std::string s = "hi";  s += "!";
来源：http://hz.ehwqpu.com/gtsvmrpnyk.html

[S33] C++：vector 增删
来源：http://hz.xylfe.cn/gtjwaldzkn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gzhubu.top/gtktxnegye.html

[S34] C++：遍历 vector
来源：http://hz.chenlongwang.top/gtefqrraha.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xylfe.cn/gtmgjfqbjs.html

[S35] C++：map
来源：http://hz.jqgfzy.top/gtidvatfqu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtpumfvkiz.html

[S36] C++：unordered_map
来源：http://hz.smart0.xyz/gtcropzllt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sweek.top/gtekddtttn.html

[S37] C++：set
来源：http://hz.wangshuangyany.cn/gtwrvwigoj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yanxiufei.cn/gtyrwhioif.html

[S38] C++：排序
来源：http://hz.ybcxt.top/gtjwyiodqh.html

std::sort(v.begin(), v.end());
来源：http://hz.svipenyu.cn/gtppmqgzen.html

[S39] C++：自定义比较器排序
来源：http://hz.gogol.net.cn/gtnwqrznxp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gaohongyu789.top/gtzednbvil.html

[S40] C++：查找元素
来源：http://hz.chenlongwang.top/gtzhjstjdv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shanyushiyangtech.top/gtucdbnedb.html

[S41] C++：类与构造函数
来源：http://hz.pycfn.com/gtkseoxtln.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.havefunace.top/gtcpswplmu.html

[S42] C++：继承与虚函数
来源：http://hz.xinyue.icu/gtpwaclbfw.html

class B : public Base { public: void f() override {} };
来源：http://hz.yvedp.cn/gtgnqhdavk.html

[S43] C++：智能指针
来源：http://hz.ydzc1.top/gtydknkdpf.html

auto p = std::make_unique<int>(5);
来源：http://hz.redwolf501.top/gtcfbbqnwe.html

[S44] C++：引用传参
来源：http://hz.hysaishi.cn/gtrrpkzkga.html

void inc(int &x) { ++x; }
来源：http://hz.cqqwz.cn/gtlbibecls.html

[S45] C++：lambda
来源：http://hz.zhiwuduotai.top/gtomcgvxdw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ywan-chungtsiang.top/gtblmmtork.html

[S46] C++：函数模板
来源：http://hz.feifeiyinyue.top/gtobrewrfi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jiagoushi.top/gtbhanyjfo.html

[S47] C++：结构化绑定遍历
来源：http://hz.hongshengwenyu.top/gtjxlugdmp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.c1oappe.top/gtyxgrfecl.html

[S48] C++：逐行读文件
来源：http://hz.iojbl.cn/gtybgtllpq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.nanxinkj.top/gtsrsdcylq.html

while (std::getline(in, line)) { }
来源：http://hz.fengsongda.top/gtxbhhydsn.html

[S49] C++：写文件
来源：http://hz.jianghu66.top/gtyypierol.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.pycfn.com/gtxujlyszk.html

[S50] C++：格式化数字
来源：http://hz.ydjk.org.cn/gtmihtnynk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinghuilouyu.cn/gtgciugfop.html

[S51] C++：显式类型转换
来源：http://hz.tianlin.xyz/gtbotrpkfm.html

static_cast<double>(a) / b
来源：http://hz.redwolf501.top/gtnzfxodaq.html

[S52] C++：const 与 noexcept
来源：http://hz.hnxiangtu.top/gtlpzdjewq.html

int size() const noexcept { return n_; }
来源：http://hz.316326.xyz/gtpccziudj.html

[S53] C++：移动语义
来源：http://hz.kuanghao11.cn/gtkoncmrdq.html

std::vector<int> w = std::move(v);
来源：http://hz.andypj.xyz/gtgovofect.html

[S54] C++：异常处理
来源：http://hz.daria6918.cn/gtnqkynnci.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yuxming.cn/gtibilfmvu.html

[S55] C++：结构化绑定
来源：http://hz.kuanghao11.cn/gtzirrdcke.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.feifeiyinyue.top/gtbqeigmhy.html

[S56] C++：optional
来源：http://hz.gogol.net.cn/gtcnjqaoqv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yangfankeji.com/gtwaiavhfq.html

[S57] C++：编译期常量
来源：http://hz.cdnleiting.top/gtqeucyzku.html

constexpr int N = 10;
来源：http://hz.ydzc1.top/gtawromewv.html

[S58] C++：命名空间
来源：http://hz.jiagoushi.top/gtbkoxnvjx.html

namespace ns { int f() { return 1; } }
来源：http://hz.guannengcc.top/gtsycuglpv.html

[S59] C++：静态断言
来源：http://hz.ivvv.top/gtplizhqnh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jianghu66.top/gtbahwkyfu.html

[S60] C++：遍历并删除元素
来源：http://hz.zycfv.cn/gtizaxidsn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.0kj1m.cn/gtogffszhs.html

================================================================================
来源：http://hz.hywenlv.cn/gtnpechoxz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pengpengdd.cyou/gtmdxecgzx.html

================================================================================
来源：http://hz.yj202588.top/gtbfiycnjx.html

[T01] Kotlin：Hello World
来源：http://hz.gogol.net.cn/gtpjvznhgn.html

println("Hello")
来源：http://hz.0kj1m.cn/gtvbjiidwi.html

[T02] Kotlin：变量
来源：http://hz.cheryme.top/gtvlfkqrkp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yongpay.top/gtnytaawgp.html

[T03] Kotlin：字符串模板
来源：http://hz.nanxinkj.top/gtalsxxcyc.html

"值: $b"
来源：http://hz.daxiang520.top/gtuqsjdxyv.html

[T04] Kotlin：空安全
来源：http://hz.sxryk.cn/gtlppxqdqd.html

val n: String? = null;  n?.length
来源：http://hz.hammf.cn/gtoxvyeagy.html

[T05] Kotlin：when 表达式
来源：http://hz.sysykeji.top/gthleuzvyi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhoulong.xyz/gtzhutmgrt.html

[T06] Kotlin：集合映射
来源：http://hz.52xcode.cn/gtodlbjwgy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jiagoushi.top/gthkohtjzf.html

[T07] Kotlin：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtqflraspo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuxming.cn/gthkipegqq.html

[T08] Kotlin：数据类
来源：http://hz.chenlongwang.top/gtkrltzwwz.html

data class User(val name: String, val age: Int)
来源：http://hz.ivvv.top/gtujtnmwuj.html

[T09] Kotlin：扩展函数
来源：http://hz.cashguo.top/gtnidubtkr.html

fun String.exclaim() = this + "!"
来源：http://hz.shanyushiyangkeji.top/gtftbvcyfu.html

[T10] Kotlin：默认参数
来源：http://hz.guannengcc.top/gtyjqmhrrn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.snrcjt.cn/gtncvsbdyz.html

[T11] Kotlin：协程
来源：http://hz.shuidangran.top/gtcwhcyfra.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.redwolf501.top/gtsymycisz.html

[T12] Kotlin：解构声明
来源：http://hz.sysykeji.top/gtvkwwqdqp.html

val (a, b) = Pair(1, 2)
来源：http://hz.hysaishi.cn/gtkfcpvcws.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtglhavalm.html

val m = mapOf("a" to 1)
来源：http://hz.yanxiufei.cn/gtebkgnhiq.html

[T14] Kotlin：循环
来源：http://hz.zhengqikj.top/gtaacsyays.html

for (i in 1..10) println(i)
来源：http://hz.kuanghao11.cn/gttmtwdvwq.html

[T15] Kotlin：接口
来源：http://hz.jinyuanbaomall.cn/gtunwqnlja.html

interface Shape { fun area(): Double }
来源：http://hz.meibo888.top/gtnyxxouyw.html

[T16] Swift：Hello World
来源：http://hz.yuxming.cn/gtxwzdapbi.html

print("Hello")
来源：http://hz.jiagoushi.top/gtlcrmlfvm.html

[T17] Swift：变量与常量
来源：http://hz.cqqwz.cn/gttsxmgvqr.html

var a = 1;  let b = 2
来源：http://hz.jlsjyb.cn/gtdiacnrat.html

[T18] Swift：字符串插值
来源：http://hz.jiagoushi.top/gtmprzoigx.html

"值: \(b)"
来源：http://hz.hongshengwenyu.top/gthbapbzqb.html

[T19] Swift：可选绑定
来源：http://hz.haohaochexian.top/gtzqomxesb.html

if let n = opt { print(n) }
来源：http://hz.birdmap.top/gtddlysswc.html

[T20] Swift：数组操作
来源：http://hz.daria6918.cn/gtjdmdxury.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yangfankeji.com/gtzytgmfuv.html

[T21] Swift：遍历
来源：http://hz.zhengqikj.top/gttjgzlcll.html

for x in a { print(x) }
来源：http://hz.jinqigfzy.top/gtshditskq.html

[T22] Swift：字典
来源：http://hz.bjfxy.top/gtebqmkxgd.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jiagoushi.top/gtnvfvbsrm.html

[T23] Swift：函数
来源：http://hz.316326.xyz/gtuqbduvnt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.birdmap.top/gtfxhesitu.html

[T24] Swift：闭包
来源：http://hz.shzxlz.cn/gtcsxkftyb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenzaomai.com/gtqozyrqwi.html

[T25] Swift：结构体
来源：http://hz.ehwqpu.com/gtpbnvcihq.html

struct P { var x: Int }
来源：http://hz.aibaodan.cn/gtkisfvyxr.html

[T26] Swift：类与重写
来源：http://hz.jlsjyb.cn/gtiagtnath.html

class A: Base { override func f() {} }
来源：http://hz.cqqwz.cn/gtuqljioax.html

[T27] Swift：错误处理
来源：http://hz.jianghu66.top/gtmjhyzdhq.html

do { try f() } catch { print(error) }
来源：http://hz.nwbrower.top/gtyxoyswxn.html

[T28] Swift：枚举
来源：http://hz.yanxiufei.cn/gtgdljogjd.html

enum Color { case red, green }
来源：http://hz.jinqigfzy.top/gtdaxfzrhy.html

[T29] Swift：guard 提前返回
来源：http://hz.ywan-chungtsiang.top/gtqokhnwyc.html

guard let x = opt else { return }
来源：http://hz.zhongyouzk.top/gtwpctmuul.html

[T30] Swift：协议
来源：http://hz.gzhubu.top/gtauglhqgc.html

protocol Shape { func area() -> Double }
来源：http://hz.tian-w.cn/gtqhzdlqlc.html

[T31] Lua：Hello World
来源：http://hz.yangfankeji.com/gtuvfaumto.html

print("Hello")
来源：http://hz.zhengqikj.top/gtvuxtlbnb.html

[T32] Lua：局部变量
来源：http://hz.9152youxi.cn/gthophcyjd.html

local a = 1
来源：http://hz.vqdsnc.cn/gtpkmyovrg.html

[T33] Lua：表（数组）
来源：http://hz.wangshuangyany.cn/gtubutmxzt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cucudq.cn/gttlacywqp.html

[T34] Lua：遍历表
来源：http://hz.shzxlz.cn/gtspbosevq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jqgufenzy.top/gtczafzkfy.html

[T35] Lua：字典表
来源：http://hz.vqdsnc.cn/gtsgehqxvp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yongpay.top/gtvujorqyn.html

[T36] Lua：函数
来源：http://hz.chenzaomai.com/gtnamaxaon.html

function add(a, b) return a + b end
来源：http://hz.tanke756.top/gtyazohqpr.html

[T37] Lua：字符串拼接
来源：http://hz.zhiwuduotai.top/gtxflbptuz.html

"a" .. "b"
来源：http://hz.shuidangran.top/gttqwelush.html

[T38] Lua：条件
来源：http://hz.yj20258888.top/gtmomlxbfu.html

if x > 0 then print("正") end
来源：http://hz.quarkkingdee.top/gtzehyhvwc.html

[T39] Lua：模式匹配
来源：http://hz.xingfuxueyuan.xyz/gtwqkfaelr.html

string.find(s, "%d+")
来源：http://hz.yj20258888.top/gtcsdztcxg.html

[T40] Lua：元表
来源：http://hz.zhoulong.xyz/gtufmmndlu.html

setmetatable({}, { __index = base })
来源：http://hz.fengsongda.top/gtashrzqhh.html

[T41] Perl：Hello World
来源：http://hz.fzhhl.top/gtyhibocmq.html

print "Hello\n";
来源：http://hz.jinqigfzy.top/gtjncorepw.html

[T42] Perl：变量类型
来源：http://hz.yj20258.top/gtmlokcwcc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zdqjudy.top/gtktmepcxl.html

[T43] Perl：字符串插值
来源：http://hz.sxryk.cn/gtbpugtidw.html

"值: $a"
来源：http://hz.zhengqikj.top/gtdabxryvp.html

[T44] Perl：条件
来源：http://hz.jyoumei.cn/gtvblfhwpb.html

if ($a > 0) { print "正"; }
来源：http://hz.hnqzz.top/gttajsnlbn.html

[T45] Perl：数组遍历
来源：http://hz.zhixingplan.top/gtrqyqdzox.html

for my $x (@arr) { print $x; }
来源：http://hz.dianchejie.cn/gtlpcqekvu.html

[T46] Perl：哈希操作
来源：http://hz.shanyushiyangtech.top/gtlgppgffi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shangyingyoupin.top/gtsjkdrykv.html

[T47] Perl：正则捕获
来源：http://hz.sweek.top/gtaozaosfw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.redwolf501.top/gtgowbtlfe.html

[T48] Perl：正则替换
来源：http://hz.yanxiufei.cn/gtbomotolb.html

$s =~ s/old/new/g;
来源：http://hz.zhiwuduotai.top/gtrssreimt.html

[T49] Perl：函数
来源：http://hz.zycfv.cn/gtzrfukdio.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.iojbl.cn/gtwjuhzlxb.html

[T50] Perl：逐行读文件
来源：http://hz.52xcode.cn/gtdnxmufpc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tian-w.cn/gtjuclspra.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.sufxvd.cn/gtzyvhaxsr.html

[T51] Scala：Hello World
来源：http://hz.chenlongwang.top/gtpxuztvjx.html

println("Hello")
来源：http://hz.svipenyu.cn/gtvfsscuzz.html

[T52] Scala：变量
来源：http://hz.zhoulong.xyz/gttejmgmfp.html

val a = 1;  var b = 2
来源：http://hz.haohaochexian.top/gtlvwrhcvw.html

[T53] Scala：字符串插值
来源：http://hz.chenzaomai.com/gtpnrkelvx.html

s"值: $b"
来源：http://hz.guannengcc.top/gtdxrwwcxv.html

[T54] Scala：集合映射
来源：http://hz.daria6918.cn/gtrnolrnko.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.nanxinkj.top/gtarysmdbz.html

[T55] Scala：集合过滤
来源：http://hz.snrcjt.cn/gtsvktghpw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jqgfzy.top/gtgreqzimd.html

[T56] Scala：样例类
来源：http://hz.ywan-chungtsiang.top/gtalfvoems.html

case class User(name: String, age: Int)
来源：http://hz.chenjidiqi.icu/gtavfvgdgd.html

[T57] Scala：模式匹配
来源：http://hz.cdnleiting.top/gtftxpylpo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.chenjidiqi.icu/gtpvfhcbwj.html

[T58] Scala：函数定义
来源：http://hz.ywan-chungtsiang.top/gttxzveoaj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ppjwa.cn/gtynhuhcgf.html

[T59] Scala：循环
来源：http://hz.chenjidiqi.icu/gtcwokppig.html

for (i <- 1 to 10) println(i)
来源：http://hz.jyoumei.cn/gtdhhrqigv.html

[T60] Scala：折叠
来源：http://hz.andypj.xyz/gttnllnhrx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.aizwys.cn/gtmqtxrutg.html

================================================================================
来源：http://hz.9152youxi.cn/gtoqermjag.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xziqi.cn/gtbxgabhat.html

================================================================================
来源：http://hz.shzxlz.cn/gtzlcrxscb.html

[U01] Py：创建虚拟环境
来源：http://hz.316326.xyz/gtajeuuduh.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tian-w.cn/gthmraoizc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.vqdsnc.cn/gtreyrtxjn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhaomingkeji.xyz/gtjdejcrwm.html

[U03] Py：加载 .env 配置
来源：http://hz.kuanghao11.cn/gtjkglartm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.svipenyu.cn/gthdjpcats.html

[U04] Py：变量调试打印
来源：http://hz.jinqigufen.top/gtgulskopw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jianghu66.top/gtshhslcte.html

[U05] Py：列表去重且保序
来源：http://hz.yueranfly.top/gtskkwvxsj.html

list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtnkutjous.html

[U06] Py：合并两个字典
来源：http://hz.gzhubu.top/gtjxufbryz.html

{**a, **b}
来源：http://hz.zhoulong.xyz/gthucffinz.html

[U07] Py：反转字典键值
来源：http://hz.zhixingplan.top/gtpbxgjhtp.html

{v: k for k, v in d.items()}
来源：http://hz.nanxuanxn.top/gtohxtzigr.html

[U08] Py：展平二维列表
来源：http://hz.yanxiufei.cn/gtiqdmgapf.html

[y for x in nested for y in x]
来源：http://hz.yj20258.top/gtzkxbntfw.html

[U09] Py：字典取最大值的键
来源：http://hz.vqdsnc.cn/gtsnxsfdxp.html

max(d, key=d.get)
来源：http://hz.smart0.xyz/gtisyipoha.html

[U10] Py：按值排序字典
来源：http://hz.tianlin.xyz/gthljetllz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.shuidangran.top/gtmzhkqmld.html

[U11] Py：生成器表达式
来源：http://hz.haohaochexian.top/gtailipfnh.html

(x * 2 for x in arr)
来源：http://hz.0kj1m.cn/gtvygxcsfy.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhoulong.xyz/gtvutanpju.html

Counter(arr).most_common(3)
来源：http://hz.xuetiantiany.cn/gtxotakjrq.html

[U13] Py：固定长度队列
来源：http://hz.tanke756.top/gttmpdrzsx.html

deque(maxlen=10)
来源：http://hz.ydjk.org.cn/gtmcxzbphx.html

[U14] Py：分组收集到列表
来源：http://hz.yangfankeji.com/gtktpynfxu.html

defaultdict(list)
来源：http://hz.jlsjyb.cn/gtzwnqcijk.html

[U15] Py：高精度计时
来源：http://hz.daxiang520.top/gtdefoxavb.html

t = time.perf_counter()
来源：http://hz.hysaishi.cn/gtikyvnqjw.html

[U16] Py：命令行参数解析
来源：http://hz.ivvv.top/gtdzsetorm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cheryme.top/gtzsgbhwlz.html

[U17] Py：初始化日志
来源：http://hz.shzxlz.cn/gtuufoemfs.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhiwuduotai.top/gtdiaufxbe.html

[U18] Py：预编译正则
来源：http://hz.shanyushiyangkeji.top/gtlgcusxtf.html

pat = re.compile(r"\d+")
来源：http://hz.shangyingyoupin.top/gtdqjkxklj.html

[U19] Py：正则替换带回调
来源：http://hz.jqgufenzy.top/gtxjpjrqcx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cucudq.cn/gtaxpgyxvc.html

[U20] Py：缓存函数结果
来源：http://hz.shuidangran.top/gtzaaegecm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhoulong.xyz/gthcvnfxok.html

[U21] Py：自定义上下文管理器
来源：http://hz.jqgufenzy.top/gtcgdyvsqf.html

@contextlib.contextmanager
来源：http://hz.chenzaomai.com/gtdvjhthsy.html

[U22] Py：矩阵转置
来源：http://hz.ppjwa.cn/gtgaflfipu.html

list(zip(*m))
来源：http://hz.nwbrower.top/gtxkabjqdk.html

[U23] Py：分块读取大文件
来源：http://hz.sysykeji.top/gtsgphjvhm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gotoacloud.top/gtislsefcr.html

[U24] Py：路径操作
来源：http://hz.tian-w.cn/gtcxbwyrzi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenjidiqi.icu/gtonnojjtx.html

[U25] Py：CSV 按字典读
来源：http://hz.wangdashe.top/gtvwyibclm.html

csv.DictReader(f)
来源：http://hz.jqgufenzy.top/gtutfejsqj.html

[U26] Py：并发下载
来源：http://hz.pycfn.com/gtwvxzijac.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.dianchejie.cn/gtclnzbbpa.html

[U27] Py：异步 HTTP
来源：http://hz.mhx1999.top/gtlvshezjc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinghuilouyu.cn/gtdnkxmvdi.html

[U28] Py：类型别名
来源：http://hz.smart0.xyz/gtkkumbisu.html

UserId = int
来源：http://hz.meibo888.top/gtvnwvgous.html

[U29] Py：属性校验
来源：http://hz.c1oappe.top/gtwvytcjgp.html

@property 与 @x.setter 配合
来源：http://hz.jlsjyb.cn/gtuefftegd.html

[U30] Py：数据类
来源：http://hz.hnxiangtu.top/gtbxchkuhx.html

@dataclass(slots=True)
来源：http://hz.chenjidiqi.icu/gtatevtlfe.html

[U31] Py：单测
来源：http://hz.yueranfly.top/gtnuvdjsjw.html

python -m pytest -q
来源：http://hz.yj20258888.top/gtbjmrrvwa.html

[U32] Py：代码格式化
来源：http://hz.9152youxi.cn/gtynucmxcw.html

ruff format . && ruff check --fix .
来源：http://hz.meibo888.top/gtmddvwqcr.html

[U33] Py：打包发布
来源：http://hz.feifeiyinyue.top/gtznjctrxv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ydzc1.top/gtloabxlud.html

[U34] Py：判断编码
来源：http://hz.redwolf501.top/gttilwqvrx.html

chardet.detect(raw)
来源：http://hz.cqqwz.cn/gtiozrbubi.html

[U35] Py：发送邮件
来源：http://hz.316326.xyz/gtawuslvdb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ydzc1.top/gtbfkzvrdw.html

[U36] Py：定时任务
来源：http://hz.yueranfly.top/gtwrapsmxp.html

schedule.every(10).minutes.do(job)
来源：http://hz.xuetiantiany.cn/gtjvbcawoj.html

[U37] Py：读写 Excel
来源：http://hz.cdnleiting.top/gtyjabobuo.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.mhx1999.top/gthseexdwi.html

[U38] Py：获取脚本所在目录
来源：http://hz.yj20258888.top/gtealxzvaj.html

Path(__file__).resolve().parent
来源：http://hz.dianchejie.cn/gtjkubhzwe.html

[U39] Py：判断是否在交互环境
来源：http://hz.daria6918.cn/gtvtesnwxy.html

sys.stdout.isatty()
来源：http://hz.ppjwa.cn/gtlatvxkvq.html

[U40] Py：打印到标准错误
来源：http://hz.jqgfzy.top/gtxqtscnsq.html

print("err", file=sys.stderr)
来源：http://hz.zhengqikj.top/gtgyhunixj.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.tianlin.xyz/gtwxukqegi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.tian-w.cn/gtetzotccu.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.aibaodan.cn/gtrqgzpomj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.havefunace.top/gtwyykhazb.html

[U43] PHP：声明命名空间
来源：http://hz.hfpthk.cn/gtigcdjqeg.html

namespace App\Http;
来源：http://hz.yvedp.cn/gtfofaucqg.html

[U44] PHP：开启严格类型
来源：http://hz.birdmap.top/gtqfzmrmey.html

declare(strict_types=1);
来源：http://hz.cheryme.top/gtyxhnmzmi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yj20258.top/gtnxvevrte.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtzbygnmmz.html

[U46] PHP：可空类型
来源：http://hz.jiagoushi.top/gtqadnefut.html

?string $name = null
来源：http://hz.meibo888.top/gtnlrjyufq.html

[U47] PHP：联合类型
来源：http://hz.nanxinkj.top/gtzctcqsfb.html

int|string $id
来源：http://hz.wangdashe.top/gtrxoxxsmb.html

[U48] PHP：纯枚举
来源：http://hz.tian-w.cn/gtxkwgwvrt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hongshengwenyu.top/gthvefkyyl.html


<!-- 参考信息 -->