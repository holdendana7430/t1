代发 wailian999

#ifndef X_H
来源：http://hz.tianlin.xyz/gtiqxckjlt.html

#define X_H
来源：http://hz.jinghuilouyu.cn/gtepbgnnnw.html

#endif
来源：http://hz.dashuyun.cn/gtwmlkeiqp.html

[S31] C++：Hello World
来源：http://hz.ppjwa.cn/gtlcqazhdd.html

#include <iostream>
来源：http://hz.yuanzhike.top/gttxvafvgs.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.birdmap.top/gttixmuftd.html

[S32] C++：字符串
来源：http://hz.dashuyun.cn/gtrdmomtxy.html

std::string s = "hi";  s += "!";
来源：http://hz.ivvv.top/gtzyumbpcd.html

[S33] C++：vector 增删
来源：http://hz.guannengcc.top/gtwwccswqu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hywenlv.cn/gttbbahyig.html

[S34] C++：遍历 vector
来源：http://hz.cucudq.cn/gtsyrwekmp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sysykeji.top/gtfqdbigpx.html

[S35] C++：map
来源：http://hz.dashuyun.cn/gtrukqneoe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtjzvthhuk.html

[S36] C++：unordered_map
来源：http://hz.jinghuilouyu.cn/gtyjrnxiel.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtnzhdnffq.html

[S37] C++：set
来源：http://hz.fengsongda.top/gtlwjrveaw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aibaodan.cn/gtghuxajnz.html

[S38] C++：排序
来源：http://hz.guannengcc.top/gtealnbaqh.html

std::sort(v.begin(), v.end());
来源：http://hz.guowangkeji.top/gthbzwpuzt.html

[S39] C++：自定义比较器排序
来源：http://hz.mhx1999.top/gtbhsdjqif.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sysykeji.top/gtltmmbgbm.html

[S40] C++：查找元素
来源：http://hz.xuanzx.com/gtdxkmwxjn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hywenlv.cn/gtiuwjshxf.html

[S41] C++：类与构造函数
来源：http://hz.daxiang520.top/gtvzltdcqw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.9152youxi.cn/gteeceonbb.html

[S42] C++：继承与虚函数
来源：http://hz.sufxvd.cn/gtqikkjmkr.html

class B : public Base { public: void f() override {} };
来源：http://hz.shangyingyoupin.top/gtcwikgmsf.html

[S43] C++：智能指针
来源：http://hz.gogol.net.cn/gtanggcwia.html

auto p = std::make_unique<int>(5);
来源：http://hz.aibaodan.cn/gtaywowyik.html

[S44] C++：引用传参
来源：http://hz.jinyuanbaomall.cn/gtchrsjmol.html

void inc(int &x) { ++x; }
来源：http://hz.xuanzx.com/gtocrauukv.html

[S45] C++：lambda
来源：http://hz.meibo888.top/gtsrvhbieg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinqigufen.top/gtojbsbbrm.html

[S46] C++：函数模板
来源：http://hz.yuxming.cn/gtxwyhfmri.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.dashuyun.cn/gtionawlxe.html

[S47] C++：结构化绑定遍历
来源：http://hz.nwbrower.top/gtvnajanui.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gotoacloud.top/gtkaluguwf.html

[S48] C++：逐行读文件
来源：http://hz.gogol.net.cn/gtcjfzuysv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.9152youxi.cn/gttmtigbni.html

while (std::getline(in, line)) { }
来源：http://hz.chenlongwang.top/gtuaciwonc.html

[S49] C++：写文件
来源：http://hz.cheryme.top/gtsnftqrwy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sufxvd.cn/gthkqctspt.html

[S50] C++：格式化数字
来源：http://hz.c1oappe.top/gtkbnzunsw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj202588.top/gtgtuhqygp.html

[S51] C++：显式类型转换
来源：http://hz.yuxming.cn/gttyikqubt.html

static_cast<double>(a) / b
来源：http://hz.xingfuxueyuan.xyz/gtrreirlkd.html

[S52] C++：const 与 noexcept
来源：http://hz.birdmap.top/gtopmrwkpc.html

int size() const noexcept { return n_; }
来源：http://hz.shzxlz.cn/gtugbghjlo.html

[S53] C++：移动语义
来源：http://hz.tian-w.cn/gtooudbfwq.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigufen.top/gtegglkqro.html

[S54] C++：异常处理
来源：http://hz.bjfxy.top/gtcorbhdli.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhiwuduotai.top/gtzhfwiiuy.html

[S55] C++：结构化绑定
来源：http://hz.guowangkeji.top/gtuoejymph.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenzaomai.com/gtrtiwhyww.html

[S56] C++：optional
来源：http://hz.yanxiufei.cn/gtzvrgxtkp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgufenzy.top/gtlkhkslth.html

[S57] C++：编译期常量
来源：http://hz.xziqi.cn/gtxftkxhkq.html

constexpr int N = 10;
来源：http://hz.tianlin.xyz/gtzgdpvdso.html

[S58] C++：命名空间
来源：http://hz.tianlin.xyz/gtidgkkaff.html

namespace ns { int f() { return 1; } }
来源：http://hz.hysaishi.cn/gtkpvmrfge.html

[S59] C++：静态断言
来源：http://hz.jinqigfzy.top/gtfziwwntx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gaohongyu789.top/gtyyinodds.html

[S60] C++：遍历并删除元素
来源：http://hz.ehwqpu.com/gtwedvlyop.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhijiandao.cn/gtmtfjxrmb.html

================================================================================
来源：http://hz.hnxiangtu.top/gtawgepuyi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258.top/gtqwijaprp.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmmprcjbo.html

[T01] Kotlin：Hello World
来源：http://hz.jinghuilouyu.cn/gtlhmytgmb.html

println("Hello")
来源：http://hz.jqgfzy.top/gtprmqdbbg.html

[T02] Kotlin：变量
来源：http://hz.haohaochexian.top/gtantqqmzn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jyoumei.cn/gtiujpezpo.html

[T03] Kotlin：字符串模板
来源：http://hz.zhoulong.xyz/gtccyukqfi.html

"值: $b"
来源：http://hz.zdqjudy.top/gtwhvqysvz.html

[T04] Kotlin：空安全
来源：http://hz.havefunace.top/gttsqtkfif.html

val n: String? = null;  n?.length
来源：http://hz.hongshengwenyu.top/gtdghvuvbf.html

[T05] Kotlin：when 表达式
来源：http://hz.yuanzhike.top/gtnktfhepu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.birdmap.top/gtzygnapxk.html

[T06] Kotlin：集合映射
来源：http://hz.shanyushiyangtech.top/gtqumbdjtw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangshuangyany.cn/gtenfoeoon.html

[T07] Kotlin：集合过滤
来源：http://hz.hfpthk.cn/gtgdnnkwlw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhoulong.xyz/gtabvrsfzj.html

[T08] Kotlin：数据类
来源：http://hz.xuanzx.com/gtxochujse.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gtcetbozqn.html

[T09] Kotlin：扩展函数
来源：http://hz.hongshengwenyu.top/gtzumrhwci.html

fun String.exclaim() = this + "!"
来源：http://hz.hnxiangtu.top/gtqgqfmncc.html

[T10] Kotlin：默认参数
来源：http://hz.ydzc1.top/gtnwpvpiyv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aizwys.cn/gtlgtjwxyu.html

[T11] Kotlin：协程
来源：http://hz.yanxiufei.cn/gtxbkaidpn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.pycfn.com/gtduatsqks.html

[T12] Kotlin：解构声明
来源：http://hz.gaohongyu789.top/gtnkwtkuwc.html

val (a, b) = Pair(1, 2)
来源：http://hz.jlsjyb.cn/gtzuxgovfg.html

[T13] Kotlin：只读 Map
来源：http://hz.dashuyun.cn/gtiomyhsti.html

val m = mapOf("a" to 1)
来源：http://hz.havefunace.top/gtavhpvskf.html

[T14] Kotlin：循环
来源：http://hz.jinqigfzy.top/gtjwwzpcir.html

for (i in 1..10) println(i)
来源：http://hz.shzxlz.cn/gtglhftraj.html

[T15] Kotlin：接口
来源：http://hz.yueranfly.top/gtlkyoertl.html

interface Shape { fun area(): Double }
来源：http://hz.shanyushiyangkeji.top/gtdnwfuopq.html

[T16] Swift：Hello World
来源：http://hz.yueranfly.top/gthynktmvu.html

print("Hello")
来源：http://hz.xuanzx.com/gtxuklcevv.html

[T17] Swift：变量与常量
来源：http://hz.kuanghao11.cn/gtucuzrerz.html

var a = 1;  let b = 2
来源：http://hz.ydzc1.top/gtcpnxqxkz.html

[T18] Swift：字符串插值
来源：http://hz.tianlin.xyz/gtvwfpthvs.html

"值: \(b)"
来源：http://hz.yuxming.cn/gtmwywfinm.html

[T19] Swift：可选绑定
来源：http://hz.yuanzhike.top/gtuycfehwf.html

if let n = opt { print(n) }
来源：http://hz.haohaochexian.top/gtzuwhxjth.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtlkxdubmg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gzhubu.top/gtraosaxvz.html

[T21] Swift：遍历
来源：http://hz.vqdsnc.cn/gtpaveielo.html

for x in a { print(x) }
来源：http://hz.sweek.top/gtaimoaprg.html

[T22] Swift：字典
来源：http://hz.hammf.cn/gtjcsmijhc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.c1oappe.top/gtjglnvwol.html

[T23] Swift：函数
来源：http://hz.zhoulong.xyz/gttauczvqp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sysykeji.top/gttfsjaifs.html

[T24] Swift：闭包
来源：http://hz.jinqigfzy.top/gtzrlbwuos.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.iojbl.cn/gthsttirmp.html

[T25] Swift：结构体
来源：http://hz.sxryk.cn/gtvbztpjip.html

struct P { var x: Int }
来源：http://hz.guowangkeji.top/gtobznvxdy.html

[T26] Swift：类与重写
来源：http://hz.andypj.xyz/gtlupkrixf.html

class A: Base { override func f() {} }
来源：http://hz.havefunace.top/gtexcrpkfn.html

[T27] Swift：错误处理
来源：http://hz.jyoumei.cn/gtvreiyqhg.html

do { try f() } catch { print(error) }
来源：http://hz.xuetiantiany.cn/gtwgrtiogw.html

[T28] Swift：枚举
来源：http://hz.bjfxy.top/gttwpdtotm.html

enum Color { case red, green }
来源：http://hz.chenlongwang.top/gtuerkvass.html

[T29] Swift：guard 提前返回
来源：http://hz.cheryme.top/gtkarmpwjw.html

guard let x = opt else { return }
来源：http://hz.chenjidiqi.icu/gtgiehnwan.html

[T30] Swift：协议
来源：http://hz.nwbrower.top/gtnzabsjob.html

protocol Shape { func area() -> Double }
来源：http://hz.jyoumei.cn/gtwygfsxaw.html

[T31] Lua：Hello World
来源：http://hz.yuanzhike.top/gtoctqadga.html

print("Hello")
来源：http://hz.zhongyouzk.top/gtkzcpdxoi.html

[T32] Lua：局部变量
来源：http://hz.jinghuilouyu.cn/gtjmyvmrwj.html

local a = 1
来源：http://hz.xuanzx.com/gtjtvcmisy.html

[T33] Lua：表（数组）
来源：http://hz.zhaomingkeji.xyz/gtrnvbmdxx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.tian-w.cn/gtvmsxroxw.html

[T34] Lua：遍历表
来源：http://hz.zhoulong.xyz/gtdwylvbox.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yongpay.top/gtixndbjsy.html

[T35] Lua：字典表
来源：http://hz.jinghuilouyu.cn/gtnbapnadr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yongpay.top/gtrblsdtvd.html

[T36] Lua：函数
来源：http://hz.gogol.net.cn/gtgwohztxe.html

function add(a, b) return a + b end
来源：http://hz.nanxinkj.top/gtzhuqfsuj.html

[T37] Lua：字符串拼接
来源：http://hz.316326.xyz/gtqysqeqzh.html

"a" .. "b"
来源：http://hz.hammf.cn/gtaxfpbpfi.html

[T38] Lua：条件
来源：http://hz.hywenlv.cn/gthvqmgyll.html

if x > 0 then print("正") end
来源：http://hz.shanyushiyangkeji.top/gtgyhoamhl.html

[T39] Lua：模式匹配
来源：http://hz.jinghuilouyu.cn/gtwllenrls.html

string.find(s, "%d+")
来源：http://hz.ppjwa.cn/gtiylzswuk.html

[T40] Lua：元表
来源：http://hz.hnxiangtu.top/gteldvayfl.html

setmetatable({}, { __index = base })
来源：http://hz.guannengcc.top/gtfbdutlgi.html

[T41] Perl：Hello World
来源：http://hz.svipenyu.cn/gtzocjfgkh.html

print "Hello\n";
来源：http://hz.chenlongwang.top/gtrknmucwk.html

[T42] Perl：变量类型
来源：http://hz.jlsjyb.cn/gtgkmmbqfu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhixingplan.top/gtkjgugqna.html

[T43] Perl：字符串插值
来源：http://hz.ydzc1.top/gtcgjqadkx.html

"值: $a"
来源：http://hz.jyoumei.cn/gtgcmyxijs.html

[T44] Perl：条件
来源：http://hz.sysykeji.top/gtnsdqvlcc.html

if ($a > 0) { print "正"; }
来源：http://hz.hongshengwenyu.top/gtvdizrtwv.html

[T45] Perl：数组遍历
来源：http://hz.aibaodan.cn/gtsyeudjoj.html

for my $x (@arr) { print $x; }
来源：http://hz.tianlin.xyz/gtlunqtvpj.html

[T46] Perl：哈希操作
来源：http://hz.yonumen.top/gtdjzhlcrl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yangfankeji.com/gtjcepyslj.html

[T47] Perl：正则捕获
来源：http://hz.tianlin.xyz/gtyfsjrmgw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.316326.xyz/gtgxmsycqu.html

[T48] Perl：正则替换
来源：http://hz.xuetiantiany.cn/gtpoepucaa.html

$s =~ s/old/new/g;
来源：http://hz.iojbl.cn/gtwsjxeelg.html

[T49] Perl：函数
来源：http://hz.hfpthk.cn/gtkqfnhnxb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hnqzz.top/gtpmmpkwlm.html

[T50] Perl：逐行读文件
来源：http://hz.havefunace.top/gtjvmwkzas.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinghuilouyu.cn/gtjvavxxla.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinyuanbaomall.cn/gtuouyiqal.html

[T51] Scala：Hello World
来源：http://hz.cheryme.top/gtupkblhkd.html

println("Hello")
来源：http://hz.chenjidiqi.icu/gtzoumosak.html

[T52] Scala：变量
来源：http://hz.xingfuxueyuan.xyz/gtmegbyfww.html

val a = 1;  var b = 2
来源：http://hz.xuetiantiany.cn/gtauknoupu.html

[T53] Scala：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtthzbqccm.html

s"值: $b"
来源：http://hz.ydjk.org.cn/gtrddbmchx.html

[T54] Scala：集合映射
来源：http://hz.yj202588.top/gtqfvpqong.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.quarkkingdee.top/gteaqrppqy.html

[T55] Scala：集合过滤
来源：http://hz.haohaochexian.top/gtpunjemep.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yj20258.top/gtnxzfoltm.html

[T56] Scala：样例类
来源：http://hz.svipenyu.cn/gtnmbixpqb.html

case class User(name: String, age: Int)
来源：http://hz.zhijiandao.cn/gtoiyldbcg.html

[T57] Scala：模式匹配
来源：http://hz.hammf.cn/gtqoepcfmr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinyuanbaomall.cn/gtrycvrglm.html

[T58] Scala：函数定义
来源：http://hz.meibo888.top/gtwjntddgo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jyoumei.cn/gtfmiqqmvz.html

[T59] Scala：循环
来源：http://hz.xingfuxueyuan.xyz/gtweaazayj.html

for (i <- 1 to 10) println(i)
来源：http://hz.shanyushiyangkeji.top/gtvohzkzaq.html

[T60] Scala：折叠
来源：http://hz.yj202588.top/gtffbdewkf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.svipenyu.cn/gtmkadssrv.html

================================================================================
来源：http://hz.yj20258.top/gtlwiiuays.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xingfuxueyuan.xyz/gtsjmfmfki.html

================================================================================
来源：http://hz.aibaodan.cn/gtanhuyjpg.html

[U01] Py：创建虚拟环境
来源：http://hz.hfpthk.cn/gtmzikunvf.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.snrcjt.cn/gtpdlaeugm.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj202588.top/gtcmezbpfc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yonumen.top/gttrcpykek.html

[U03] Py：加载 .env 配置
来源：http://hz.fzhhl.top/gttsjwbcme.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tian-w.cn/gtkwigdwyw.html

[U04] Py：变量调试打印
来源：http://hz.yj20258888.top/gttxnxybdj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.guowangkeji.top/gtqodmpwmv.html

[U05] Py：列表去重且保序
来源：http://hz.316326.xyz/gtyiduddzc.html

list(dict.fromkeys(arr))
来源：http://hz.daria6918.cn/gtarctrzba.html

[U06] Py：合并两个字典
来源：http://hz.yj20258.top/gtxbwnuook.html

{**a, **b}
来源：http://hz.pengpengdd.cyou/gtkniwvabp.html

[U07] Py：反转字典键值
来源：http://hz.dashuyun.cn/gtxbmrasub.html

{v: k for k, v in d.items()}
来源：http://hz.yj20258.top/gtwentlchc.html

[U08] Py：展平二维列表
来源：http://hz.chenjidiqi.icu/gtlehtjxvg.html

[y for x in nested for y in x]
来源：http://hz.yvedp.cn/gtzkowiwra.html

[U09] Py：字典取最大值的键
来源：http://hz.guowangkeji.top/gtoewshqve.html

max(d, key=d.get)
来源：http://hz.tianlin.xyz/gtrurwttpn.html

[U10] Py：按值排序字典
来源：http://hz.tianlin.xyz/gtaewpvkaa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sufxvd.cn/gtvhzhcjdn.html

[U11] Py：生成器表达式
来源：http://hz.gzhubu.top/gtgedryjbc.html

(x * 2 for x in arr)
来源：http://hz.zycfv.cn/gtarogmvzn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hnqzz.top/gtbvxffgwt.html

Counter(arr).most_common(3)
来源：http://hz.tian-w.cn/gtdsayecuy.html

[U13] Py：固定长度队列
来源：http://hz.shanyushiyangkeji.top/gtjxcdhsyz.html

deque(maxlen=10)
来源：http://hz.cucudq.cn/gtcutbphem.html

[U14] Py：分组收集到列表
来源：http://hz.jiagoushi.top/gtdwqagdpq.html

defaultdict(list)
来源：http://hz.smart0.xyz/gtbflfebfx.html

[U15] Py：高精度计时
来源：http://hz.aizwys.cn/gtfwpzkrqz.html

t = time.perf_counter()
来源：http://hz.haohaochexian.top/gttgcbllrx.html

[U16] Py：命令行参数解析
来源：http://hz.zhongyouzk.top/gtmwovhjnp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xylfe.cn/gtzikhixvs.html

[U17] Py：初始化日志
来源：http://hz.52xcode.cn/gtsapkoruc.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jlsjyb.cn/gtmjxymaqc.html

[U18] Py：预编译正则
来源：http://hz.shangyingyoupin.top/gtkqwzquat.html

pat = re.compile(r"\d+")
来源：http://hz.guowangkeji.top/gtnjwufuhr.html

[U19] Py：正则替换带回调
来源：http://hz.hongshengwenyu.top/gtftunwdmp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yueranfly.top/gtukaubixh.html

[U20] Py：缓存函数结果
来源：http://hz.tianlin.xyz/gtusunxfod.html

@functools.lru_cache(maxsize=None)
来源：http://hz.iojbl.cn/gtgdvnaiku.html

[U21] Py：自定义上下文管理器
来源：http://hz.jqgfzy.top/gtwaebwnij.html

@contextlib.contextmanager
来源：http://hz.guannengcc.top/gtefhhvogn.html

[U22] Py：矩阵转置
来源：http://hz.zdqjudy.top/gtcldfftez.html

list(zip(*m))
来源：http://hz.pycfn.com/gtggzspejd.html

[U23] Py：分块读取大文件
来源：http://hz.sweek.top/gtxrupvmsl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jlsjyb.cn/gtzewscujr.html

[U24] Py：路径操作
来源：http://hz.tanke756.top/gtuvujhlbe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtvexlzlnn.html

[U25] Py：CSV 按字典读
来源：http://hz.sweek.top/gtslahffdo.html

csv.DictReader(f)
来源：http://hz.yvedp.cn/gtwzhymnjl.html

[U26] Py：并发下载
来源：http://hz.yuxming.cn/gtormhfkny.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.pycfn.com/gtdfhtajkg.html

[U27] Py：异步 HTTP
来源：http://hz.kuanghao11.cn/gtrpuzlwyi.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sxryk.cn/gtlxyquuqo.html

[U28] Py：类型别名
来源：http://hz.yj202588.top/gtspawjngf.html

UserId = int
来源：http://hz.ydzc1.top/gtxvomwrmg.html

[U29] Py：属性校验
来源：http://hz.zdqjudy.top/gtjrmmuguo.html

@property 与 @x.setter 配合
来源：http://hz.yuanzhike.top/gthgmhyzbp.html

[U30] Py：数据类
来源：http://hz.xylfe.cn/gtluksidhh.html

@dataclass(slots=True)
来源：http://hz.jinqigufen.top/gtasrchxlg.html

[U31] Py：单测
来源：http://hz.ydjk.org.cn/gtxeaibxbj.html

python -m pytest -q
来源：http://hz.zhongyouzk.top/gtpcntrgvz.html

[U32] Py：代码格式化
来源：http://hz.yonumen.top/gtlrjpjkkr.html

ruff format . && ruff check --fix .
来源：http://hz.yj202588.top/gtfixjndko.html

[U33] Py：打包发布
来源：http://hz.daxiang520.top/gtfekwuxlh.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ppjwa.cn/gtdbxcjzuh.html

[U34] Py：判断编码
来源：http://hz.chenjidiqi.icu/gtytbfkndo.html

chardet.detect(raw)
来源：http://hz.redwolf501.top/gtearahgkt.html

[U35] Py：发送邮件
来源：http://hz.jinghuilouyu.cn/gtpfxapatj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ydjk.org.cn/gtpdjsuusq.html

[U36] Py：定时任务
来源：http://hz.yonumen.top/gtjwnwsveg.html

schedule.every(10).minutes.do(job)
来源：http://hz.ppjwa.cn/gtbvqprfcl.html

[U37] Py：读写 Excel
来源：http://hz.zhoulong.xyz/gtctiihgmg.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinyuanbaomall.cn/gtsmcomjxu.html

[U38] Py：获取脚本所在目录
来源：http://hz.yvedp.cn/gtfhqgimkv.html

Path(__file__).resolve().parent
来源：http://hz.aizwys.cn/gtjxykfwyj.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhiwuduotai.top/gtkfjvjteq.html

sys.stdout.isatty()
来源：http://hz.jinqigfzy.top/gtantzeumj.html

[U40] Py：打印到标准错误
来源：http://hz.kuanghao11.cn/gtesbbqjlc.html

print("err", file=sys.stderr)
来源：http://hz.wangdashe.top/gtacftctkb.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.feifeiyinyue.top/gtvlxjjqdj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cashguo.top/gtjwwzfvoc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenzaomai.com/gtmtneauch.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.cashguo.top/gtijyldhkn.html

[U43] PHP：声明命名空间
来源：http://hz.yuanzhike.top/gtjpyfxrdb.html

namespace App\Http;
来源：http://hz.cdnleiting.top/gtnnzmtdxe.html

[U44] PHP：开启严格类型
来源：http://hz.shzxlz.cn/gtbhtkiibz.html

declare(strict_types=1);
来源：http://hz.zhaomingkeji.xyz/gtuzryxcbo.html

[U45] PHP：类型声明与返回类型
来源：http://hz.c1oappe.top/gtoyxwwccv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangkeji.top/gtwpcqtduq.html

[U46] PHP：可空类型
来源：http://hz.zhongyouzk.top/gttgndxgpa.html

?string $name = null
来源：http://hz.andypj.xyz/gtqrdrjyva.html

[U47] PHP：联合类型
来源：http://hz.yongpay.top/gtkbwpmnol.html

int|string $id
来源：http://hz.aizwys.cn/gtxeizztzv.html

[U48] PHP：纯枚举
来源：http://hz.hywenlv.cn/gtxemtlism.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhiwuduotai.top/gtadmnlodo.html

[U49] PHP：只读属性
来源：http://hz.yj202588.top/gtphgluvnf.html

public readonly string $name
来源：http://hz.zdqjudy.top/gtkbtupcsd.html

[U50] PHP：构造器属性提升
来源：http://hz.andypj.xyz/gtdumffcnr.html

public function __construct(private int $id) {}
来源：http://hz.tian-w.cn/gtmnubtqbw.html

[U51] PHP：数组解构
来源：http://hz.ydzc1.top/gtmqtwqpbx.html

[$a, $b] = $arr;
来源：http://hz.jianghu66.top/gtdrcgsubb.html

[U52] PHP：箭头函数
来源：http://hz.svipenyu.cn/gtliwfbxch.html

$double = fn($x) => $x * 2;
来源：http://hz.ehwqpu.com/gtzlvxexvr.html

[U53] PHP：空合并运算符
来源：http://hz.shanyushiyangtech.top/gtbnivqxqg.html

$v = $a ?? $b ?? "default";
来源：http://hz.redwolf501.top/gttbhwjpqh.html

[U54] PHP：空安全调用
来源：http://hz.yonumen.top/gtnjipjbvo.html

$obj?->method()
来源：http://hz.wangshuangyany.cn/gtllqyvmnl.html


<!-- 参考信息 -->