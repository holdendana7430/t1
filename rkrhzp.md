代发 wailian999

memset(a, 0, sizeof a);
来源：http://hz.shanyushiyangtech.top/gtuwyljwth.html

[S27] C：定义常量
来源：http://hz.zhaomingkeji.xyz/gtdprvgusi.html

const double PI = 3.14159;
来源：http://hz.nwbrower.top/gtsxlynuqz.html

[S28] C：静态变量
来源：http://hz.nanxinkj.top/gtevydurkw.html

static int counter = 0;
来源：http://hz.tianlin.xyz/gtanlntiud.html

[S29] C：变参函数
来源：http://hz.hnqzz.top/gtcsetdelz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gogol.net.cn/gtakpbjgsn.html

[S30] C：头文件保护
来源：http://hz.xinyue.icu/gtrpidmxkx.html

#ifndef X_H
来源：http://hz.9152youxi.cn/gtjthygmct.html

#define X_H
来源：http://hz.tanke756.top/gtdepudgzv.html

#endif
来源：http://hz.yj20258888.top/gtgsdsapgu.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtweltjfmb.html

#include <iostream>
来源：http://hz.cheryme.top/gtqnqkxlny.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yvedp.cn/gtvxmvtxtu.html

[S32] C++：字符串
来源：http://hz.nwbrower.top/gtepfuvvko.html

std::string s = "hi";  s += "!";
来源：http://hz.hfpthk.cn/gtwicjrfoy.html

[S33] C++：vector 增删
来源：http://hz.hywenlv.cn/gtxzhdpgvf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ydzc1.top/gtvnolsbpw.html

[S34] C++：遍历 vector
来源：http://hz.cheryme.top/gtkbabsngk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yueranfly.top/gtzqyratsf.html

[S35] C++：map
来源：http://hz.guannengcc.top/gtezabmqnu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jlsjyb.cn/gtnrdbfptw.html

[S36] C++：unordered_map
来源：http://hz.yanxiufei.cn/gtqigyvodp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.haohaochexian.top/gtlxmueycb.html

[S37] C++：set
来源：http://hz.sxryk.cn/gtlwekuioo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuanzx.com/gtqbzvybme.html

[S38] C++：排序
来源：http://hz.tanke756.top/gtwifjbyon.html

std::sort(v.begin(), v.end());
来源：http://hz.tianlin.xyz/gtuqfybkdr.html

[S39] C++：自定义比较器排序
来源：http://hz.zhoulong.xyz/gtgjxirbkc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.quarkkingdee.top/gtwjyahtyh.html

[S40] C++：查找元素
来源：http://hz.0kj1m.cn/gtzgvulniz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gaohongyu789.top/gtquhlwbnv.html

[S41] C++：类与构造函数
来源：http://hz.ivvv.top/gtcwmcairt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhoulong.xyz/gtkrmnhcaw.html

[S42] C++：继承与虚函数
来源：http://hz.sweek.top/gtbeudmtio.html

class B : public Base { public: void f() override {} };
来源：http://hz.dashuyun.cn/gtutsjixfk.html

[S43] C++：智能指针
来源：http://hz.svipenyu.cn/gtkkepxkkf.html

auto p = std::make_unique<int>(5);
来源：http://hz.xinyue.icu/gtibshpwxm.html

[S44] C++：引用传参
来源：http://hz.xziqi.cn/gtmvlfrpsk.html

void inc(int &x) { ++x; }
来源：http://hz.jqgufenzy.top/gtlfmmafms.html

[S45] C++：lambda
来源：http://hz.shanyushiyangkeji.top/gtwbwjwikp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.snrcjt.cn/gtldsqsgqn.html

[S46] C++：函数模板
来源：http://hz.yuanzhike.top/gtmmupelkd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gogol.net.cn/gtngqmdxkl.html

[S47] C++：结构化绑定遍历
来源：http://hz.xinyue.icu/gtsdzfogms.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cdnleiting.top/gtxanaqwms.html

[S48] C++：逐行读文件
来源：http://hz.ydzc1.top/gtaonlrhmr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.daxiang520.top/gtylkfnvkz.html

while (std::getline(in, line)) { }
来源：http://hz.xziqi.cn/gtobpvaaqd.html

[S49] C++：写文件
来源：http://hz.nanxinkj.top/gtbeukcvwf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenjidiqi.icu/gtkzncliud.html

[S50] C++：格式化数字
来源：http://hz.guannengcc.top/gtfnngkijz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.guowangkeji.top/gtayclvpwl.html

[S51] C++：显式类型转换
来源：http://hz.yj20258.top/gtnhduhkcc.html

static_cast<double>(a) / b
来源：http://hz.feifeiyinyue.top/gtoosaelmt.html

[S52] C++：const 与 noexcept
来源：http://hz.hysaishi.cn/gtpnmpzmnc.html

int size() const noexcept { return n_; }
来源：http://hz.fzhhl.top/gtfnxhxjvp.html

[S53] C++：移动语义
来源：http://hz.gogol.net.cn/gtpnenneel.html

std::vector<int> w = std::move(v);
来源：http://hz.shanyushiyangtech.top/gthmlnldud.html

[S54] C++：异常处理
来源：http://hz.yuanzhike.top/gtguyimkkx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.mhx1999.top/gtnsojgjhs.html

[S55] C++：结构化绑定
来源：http://hz.shanyushiyangtech.top/gtiwueqxja.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.dianchejie.cn/gtgcrtxfem.html

[S56] C++：optional
来源：http://hz.hammf.cn/gtzpilcunp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtvpozxwhn.html

[S57] C++：编译期常量
来源：http://hz.quarkkingdee.top/gtawqwikcb.html

constexpr int N = 10;
来源：http://hz.mhx1999.top/gtmpwreaqt.html

[S58] C++：命名空间
来源：http://hz.yanxiufei.cn/gtnrgtrxwo.html

namespace ns { int f() { return 1; } }
来源：http://hz.redwolf501.top/gtbnewmjgh.html

[S59] C++：静态断言
来源：http://hz.yanxiufei.cn/gtejpemlwa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhijiandao.cn/gtewvmxhxq.html

[S60] C++：遍历并删除元素
来源：http://hz.ppjwa.cn/gtxbalmvet.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cqqwz.cn/gtslymweka.html

================================================================================
来源：http://hz.gzhubu.top/gtntyzhaik.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuxming.cn/gtycogftii.html

================================================================================
来源：http://hz.sxryk.cn/gtdgpnidmi.html

[T01] Kotlin：Hello World
来源：http://hz.redwolf501.top/gtcsfulyae.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gtkdoncsyn.html

[T02] Kotlin：变量
来源：http://hz.shuidangran.top/gtdlwslwmt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zycfv.cn/gtstftemxd.html

[T03] Kotlin：字符串模板
来源：http://hz.sufxvd.cn/gtdsamksrb.html

"值: $b"
来源：http://hz.shanyushiyangtech.top/gtvbylmsrn.html

[T04] Kotlin：空安全
来源：http://hz.jinyuanbaomall.cn/gtstyisxfh.html

val n: String? = null;  n?.length
来源：http://hz.52xcode.cn/gtkmdeckmb.html

[T05] Kotlin：when 表达式
来源：http://hz.redwolf501.top/gtwedrdgot.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cheryme.top/gtksxhxaxs.html

[T06] Kotlin：集合映射
来源：http://hz.sweek.top/gtyhdoasbf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jlsjyb.cn/gtkcqqbwyd.html

[T07] Kotlin：集合过滤
来源：http://hz.dashuyun.cn/gtadfcdiaj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sysykeji.top/gtesxhhjuq.html

[T08] Kotlin：数据类
来源：http://hz.daria6918.cn/gtljmdiowu.html

data class User(val name: String, val age: Int)
来源：http://hz.c1oappe.top/gtmvzachgf.html

[T09] Kotlin：扩展函数
来源：http://hz.jinqigfzy.top/gtopmxffmo.html

fun String.exclaim() = this + "!"
来源：http://hz.jlsjyb.cn/gtxqiuysah.html

[T10] Kotlin：默认参数
来源：http://hz.yj20258888.top/gtbnxtztpb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.feifeiyinyue.top/gtvmgkwbsp.html

[T11] Kotlin：协程
来源：http://hz.ydzc1.top/gtnqjshxpc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhixingplan.top/gtbpqumbcd.html

[T12] Kotlin：解构声明
来源：http://hz.hnqzz.top/gtplwsvnqh.html

val (a, b) = Pair(1, 2)
来源：http://hz.cucudq.cn/gtbqupmjdu.html

[T13] Kotlin：只读 Map
来源：http://hz.chenjidiqi.icu/gtfrwcyrnn.html

val m = mapOf("a" to 1)
来源：http://hz.hfpthk.cn/gtqyvzrwdx.html

[T14] Kotlin：循环
来源：http://hz.zhaomingkeji.xyz/gtifvlqcmt.html

for (i in 1..10) println(i)
来源：http://hz.birdmap.top/gtiqltshsw.html

[T15] Kotlin：接口
来源：http://hz.cheryme.top/gtugeayddr.html

interface Shape { fun area(): Double }
来源：http://hz.xziqi.cn/gtgsotqoqk.html

[T16] Swift：Hello World
来源：http://hz.aizwys.cn/gtkqrvqyhr.html

print("Hello")
来源：http://hz.ydzc1.top/gtipdhujxm.html

[T17] Swift：变量与常量
来源：http://hz.birdmap.top/gtnkqmrbnp.html

var a = 1;  let b = 2
来源：http://hz.gzhubu.top/gtlgvdfgrn.html

[T18] Swift：字符串插值
来源：http://hz.ehwqpu.com/gttmumgadx.html

"值: \(b)"
来源：http://hz.yuxming.cn/gtwwkagvcv.html

[T19] Swift：可选绑定
来源：http://hz.dianchejie.cn/gtrkixruhe.html

if let n = opt { print(n) }
来源：http://hz.daxiang520.top/gtgffcvbos.html

[T20] Swift：数组操作
来源：http://hz.nanxinkj.top/gtxubjpfds.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhiwuduotai.top/gtswhtddrl.html

[T21] Swift：遍历
来源：http://hz.zhongyouzk.top/gtmtryzkiy.html

for x in a { print(x) }
来源：http://hz.hongshengwenyu.top/gtfniwaisi.html

[T22] Swift：字典
来源：http://hz.shanyushiyangkeji.top/gtljnkzalh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yanxiufei.cn/gtrqklztfg.html

[T23] Swift：函数
来源：http://hz.yonumen.top/gtceuiihbr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinghuilouyu.cn/gtreussonh.html

[T24] Swift：闭包
来源：http://hz.zdqjudy.top/gtibzrzubl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhoulong.xyz/gtdmwlwgen.html

[T25] Swift：结构体
来源：http://hz.jlsjyb.cn/gtjteidlue.html

struct P { var x: Int }
来源：http://hz.gaohongyu789.top/gthbwohbda.html

[T26] Swift：类与重写
来源：http://hz.ydzc1.top/gthbspitvb.html

class A: Base { override func f() {} }
来源：http://hz.52xcode.cn/gtlqphtyhp.html

[T27] Swift：错误处理
来源：http://hz.xingfuxueyuan.xyz/gtxmsxujcl.html

do { try f() } catch { print(error) }
来源：http://hz.hnqzz.top/gtgjptdrvk.html

[T28] Swift：枚举
来源：http://hz.xziqi.cn/gtmmvybbqd.html

enum Color { case red, green }
来源：http://hz.9152youxi.cn/gtbymaceuo.html

[T29] Swift：guard 提前返回
来源：http://hz.jinqigfzy.top/gtrbduzedr.html

guard let x = opt else { return }
来源：http://hz.cucudq.cn/gtfxwabeju.html

[T30] Swift：协议
来源：http://hz.ppjwa.cn/gtdzolujqg.html

protocol Shape { func area() -> Double }
来源：http://hz.meibo888.top/gtikyqmqns.html

[T31] Lua：Hello World
来源：http://hz.cdnleiting.top/gtkjodabpg.html

print("Hello")
来源：http://hz.gogol.net.cn/gttpjuudnn.html

[T32] Lua：局部变量
来源：http://hz.52xcode.cn/gtougzyqen.html

local a = 1
来源：http://hz.yangfankeji.com/gtudgkkwhw.html

[T33] Lua：表（数组）
来源：http://hz.ydjk.org.cn/gtagdzjqgs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hywenlv.cn/gtpzxnkpcr.html

[T34] Lua：遍历表
来源：http://hz.yj202588.top/gtbofecide.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuxming.cn/gtngglmfud.html

[T35] Lua：字典表
来源：http://hz.yj20258888.top/gtnxiuloow.html

local d = { a = 1 };  d.b = 2
来源：http://hz.snrcjt.cn/gttdhcavyb.html

[T36] Lua：函数
来源：http://hz.sufxvd.cn/gtsggkfvmb.html

function add(a, b) return a + b end
来源：http://hz.gotoacloud.top/gtdvnjbeeg.html

[T37] Lua：字符串拼接
来源：http://hz.jiagoushi.top/gtivwrccxt.html

"a" .. "b"
来源：http://hz.andypj.xyz/gtexjabqxo.html

[T38] Lua：条件
来源：http://hz.haohaochexian.top/gtosxvxazl.html

if x > 0 then print("正") end
来源：http://hz.xylfe.cn/gtliihumhd.html

[T39] Lua：模式匹配
来源：http://hz.cdnleiting.top/gtsfrrhjyv.html

string.find(s, "%d+")
来源：http://hz.ehwqpu.com/gttybyxzwf.html

[T40] Lua：元表
来源：http://hz.yuanzhike.top/gtyhnljprv.html

setmetatable({}, { __index = base })
来源：http://hz.ehwqpu.com/gtpwjwwbtm.html

[T41] Perl：Hello World
来源：http://hz.fzhhl.top/gtrbcbvjdw.html

print "Hello\n";
来源：http://hz.9152youxi.cn/gtqcpchunc.html

[T42] Perl：变量类型
来源：http://hz.zhijiandao.cn/gttmpoqurl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yuanzhike.top/gtnkyzftfo.html

[T43] Perl：字符串插值
来源：http://hz.nanxuanxn.top/gtdhvralcr.html

"值: $a"
来源：http://hz.shangyingyoupin.top/gtrdpaiesw.html

[T44] Perl：条件
来源：http://hz.chenzaomai.com/gtrbuewxwe.html

if ($a > 0) { print "正"; }
来源：http://hz.hongshengwenyu.top/gtlyvolpwm.html

[T45] Perl：数组遍历
来源：http://hz.dianchejie.cn/gthvnmnete.html

for my $x (@arr) { print $x; }
来源：http://hz.ywan-chungtsiang.top/gtodrzqiuz.html

[T46] Perl：哈希操作
来源：http://hz.snrcjt.cn/gtgnytyyzd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yuanzhike.top/gtaoycbqyb.html

[T47] Perl：正则捕获
来源：http://hz.jlsjyb.cn/gtgtswhsmx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nwbrower.top/gtzwcrjlax.html

[T48] Perl：正则替换
来源：http://hz.zhixingplan.top/gtqmidxogv.html

$s =~ s/old/new/g;
来源：http://hz.xuanzx.com/gtabfaeimr.html

[T49] Perl：函数
来源：http://hz.dianchejie.cn/gtcundzsra.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xuanzx.com/gtesctujtj.html

[T50] Perl：逐行读文件
来源：http://hz.zhengqikj.top/gtrbdcjdpr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.316326.xyz/gtzyijqxna.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shangyingyoupin.top/gtagmrypap.html

[T51] Scala：Hello World
来源：http://hz.yonumen.top/gtlqitcroc.html

println("Hello")
来源：http://hz.ydjk.org.cn/gtiwmjsgjw.html

[T52] Scala：变量
来源：http://hz.0kj1m.cn/gtcpseldpr.html

val a = 1;  var b = 2
来源：http://hz.52xcode.cn/gtmlrvrmnq.html

[T53] Scala：字符串插值
来源：http://hz.sxryk.cn/gtfttrmlkx.html

s"值: $b"
来源：http://hz.zhongyouzk.top/gttjncihgi.html

[T54] Scala：集合映射
来源：http://hz.shanyushiyangtech.top/gtqaonxthn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jyoumei.cn/gtkyqgeyds.html

[T55] Scala：集合过滤
来源：http://hz.dianchejie.cn/gtjtxlkawe.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.nanxinkj.top/gtsulyguin.html

[T56] Scala：样例类
来源：http://hz.hysaishi.cn/gtfubywmlt.html

case class User(name: String, age: Int)
来源：http://hz.cdnleiting.top/gtdtzhulti.html

[T57] Scala：模式匹配
来源：http://hz.zhiwuduotai.top/gtbpxgfkcn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yvedp.cn/gtoyfsylid.html

[T58] Scala：函数定义
来源：http://hz.jianghu66.top/gtprdqsfer.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zycfv.cn/gtpsbxzcjr.html

[T59] Scala：循环
来源：http://hz.shuidangran.top/gtgfiftryu.html

for (i <- 1 to 10) println(i)
来源：http://hz.dashuyun.cn/gtsrlhxyil.html

[T60] Scala：折叠
来源：http://hz.zhoulong.xyz/gtprbpkhwk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yueranfly.top/gtklixtuig.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gttlhyyrqq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.52xcode.cn/gtoklbqlhf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtyefaeoay.html

[U01] Py：创建虚拟环境
来源：http://hz.dashuyun.cn/gtwhbxhjxa.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ydjk.org.cn/gtqedeekud.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj20258888.top/gtkngxwsdv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.316326.xyz/gtfqcglfzl.html

[U03] Py：加载 .env 配置
来源：http://hz.yuxming.cn/gtricacmlj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.quarkkingdee.top/gtuveqasuz.html

[U04] Py：变量调试打印
来源：http://hz.jianghu66.top/gtpvvtddcu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sxryk.cn/gtigrtxjzm.html

[U05] Py：列表去重且保序
来源：http://hz.yj20258888.top/gtwxdzhugc.html

list(dict.fromkeys(arr))
来源：http://hz.meibo888.top/gtgegzxovh.html

[U06] Py：合并两个字典
来源：http://hz.jianghu66.top/gtwoskffvi.html

{**a, **b}
来源：http://hz.jianghu66.top/gtxvigiabx.html

[U07] Py：反转字典键值
来源：http://hz.yuanzhike.top/gtbeccjwaa.html

{v: k for k, v in d.items()}
来源：http://hz.zhijiandao.cn/gtyblxeomb.html

[U08] Py：展平二维列表
来源：http://hz.yueranfly.top/gthacgkrxs.html

[y for x in nested for y in x]
来源：http://hz.guowangkeji.top/gtlvszavis.html

[U09] Py：字典取最大值的键
来源：http://hz.tian-w.cn/gtqnvvzwwh.html

max(d, key=d.get)
来源：http://hz.yj20258888.top/gtahkmifgu.html

[U10] Py：按值排序字典
来源：http://hz.chenzaomai.com/gtodptubcd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hnxiangtu.top/gtpygvdcrv.html

[U11] Py：生成器表达式
来源：http://hz.meibo888.top/gttyzpkmnk.html

(x * 2 for x in arr)
来源：http://hz.sweek.top/gtubsdhubg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tanke756.top/gtlkzztxms.html

Counter(arr).most_common(3)
来源：http://hz.ywan-chungtsiang.top/gtchrlapqg.html

[U13] Py：固定长度队列
来源：http://hz.meibo888.top/gtfmcigzhk.html

deque(maxlen=10)
来源：http://hz.fengsongda.top/gtumawzvml.html

[U14] Py：分组收集到列表
来源：http://hz.quarkkingdee.top/gttxvfusha.html

defaultdict(list)
来源：http://hz.andypj.xyz/gtzvoxpfgw.html

[U15] Py：高精度计时
来源：http://hz.haohaochexian.top/gtlavvmxua.html

t = time.perf_counter()
来源：http://hz.havefunace.top/gtpxinxxlb.html

[U16] Py：命令行参数解析
来源：http://hz.shzxlz.cn/gtzshikwgg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jqgufenzy.top/gtzbkdjgor.html

[U17] Py：初始化日志
来源：http://hz.vqdsnc.cn/gthbvyapaz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yongpay.top/gtaedtsxzp.html

[U18] Py：预编译正则
来源：http://hz.vqdsnc.cn/gtewesrhnb.html

pat = re.compile(r"\d+")
来源：http://hz.cdnleiting.top/gtvxwjmnmt.html

[U19] Py：正则替换带回调
来源：http://hz.316326.xyz/gtkwqygfnr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.guannengcc.top/gtonnwumyh.html

[U20] Py：缓存函数结果
来源：http://hz.guannengcc.top/gtwlrhsfjh.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shangyingyoupin.top/gtmbtllmtu.html

[U21] Py：自定义上下文管理器
来源：http://hz.shangyingyoupin.top/gtvmybehml.html

@contextlib.contextmanager
来源：http://hz.tian-w.cn/gtjcdrpwcw.html

[U22] Py：矩阵转置
来源：http://hz.shangyingyoupin.top/gtoqwuwqvc.html

list(zip(*m))
来源：http://hz.gotoacloud.top/gtkdpnjqcy.html

[U23] Py：分块读取大文件
来源：http://hz.aibaodan.cn/gtkpvybofg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhixingplan.top/gtjmjumzfd.html

[U24] Py：路径操作
来源：http://hz.meibo888.top/gtijkxslth.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.tianlin.xyz/gttqsjtntm.html

[U25] Py：CSV 按字典读
来源：http://hz.dianchejie.cn/gtihkbveej.html

csv.DictReader(f)
来源：http://hz.xinyue.icu/gtzcecwlbh.html

[U26] Py：并发下载
来源：http://hz.jianghu66.top/gtahljaekv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.chenjidiqi.icu/gtkfnmxyzl.html

[U27] Py：异步 HTTP
来源：http://hz.nanxinkj.top/gtcumjbtsn.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.mhx1999.top/gtnrwfztxq.html

[U28] Py：类型别名
来源：http://hz.svipenyu.cn/gtcosdhxtu.html

UserId = int
来源：http://hz.vqdsnc.cn/gtdyvoptyy.html

[U29] Py：属性校验
来源：http://hz.ydjk.org.cn/gtjsbzyrca.html

@property 与 @x.setter 配合
来源：http://hz.zhongyouzk.top/gtjfqmqyai.html

[U30] Py：数据类
来源：http://hz.pengpengdd.cyou/gtzszcyjuq.html

@dataclass(slots=True)
来源：http://hz.xuanzx.com/gtkmdkglgo.html

[U31] Py：单测
来源：http://hz.snrcjt.cn/gtbtxhjsfu.html

python -m pytest -q
来源：http://hz.andypj.xyz/gtpcwbrrsz.html

[U32] Py：代码格式化
来源：http://hz.smart0.xyz/gtwxnjaqlw.html

ruff format . && ruff check --fix .
来源：http://hz.jinqigfzy.top/gtauqmgofz.html

[U33] Py：打包发布
来源：http://hz.tianlin.xyz/gtromiuvbf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.pycfn.com/gtzuhxkkkc.html

[U34] Py：判断编码
来源：http://hz.dianchejie.cn/gtspkqdurg.html

chardet.detect(raw)
来源：http://hz.guannengcc.top/gtovqhpbfm.html

[U35] Py：发送邮件
来源：http://hz.snrcjt.cn/gtyrvffgdq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cdnleiting.top/gtwthnxidv.html

[U36] Py：定时任务
来源：http://hz.jyoumei.cn/gtcufswhax.html

schedule.every(10).minutes.do(job)
来源：http://hz.ydjk.org.cn/gtfpbnxqah.html

[U37] Py：读写 Excel
来源：http://hz.birdmap.top/gtkcbgfqgj.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.meibo888.top/gtpdltadqy.html

[U38] Py：获取脚本所在目录
来源：http://hz.sysykeji.top/gtwhvlnkjz.html

Path(__file__).resolve().parent
来源：http://hz.cucudq.cn/gtvrsnkmbp.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhoulong.xyz/gtkympokcz.html

sys.stdout.isatty()
来源：http://hz.xinyue.icu/gtbhkqvbji.html

[U40] Py：打印到标准错误
来源：http://hz.chenlongwang.top/gtjggrldun.html

print("err", file=sys.stderr)
来源：http://hz.jqgfzy.top/gtzkesvafm.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jianghu66.top/gtfgpoyflm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.aibaodan.cn/gtawzvuigq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shangyingyoupin.top/gtsrhbcvwn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hywenlv.cn/gtavpnwryo.html

[U43] PHP：声明命名空间
来源：http://hz.hywenlv.cn/gtcohphpch.html

namespace App\Http;
来源：http://hz.zdqjudy.top/gtcdwsmytq.html

[U44] PHP：开启严格类型
来源：http://hz.bjfxy.top/gthzoiqcoq.html

declare(strict_types=1);
来源：http://hz.yueranfly.top/gtfdyiobkn.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhengqikj.top/gtehafwsjq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtldwmoqsf.html

[U46] PHP：可空类型
来源：http://hz.ybcxt.top/gtgbfzfuxx.html

?string $name = null
来源：http://hz.aizwys.cn/gtqrqhlrwk.html

[U47] PHP：联合类型
来源：http://hz.yuanzhike.top/gtjhadzokc.html

int|string $id
来源：http://hz.cqqwz.cn/gtbxfowtze.html

[U48] PHP：纯枚举
来源：http://hz.yj20258.top/gtpkjytwvp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xuetiantiany.cn/gtlgfonbxy.html

[U49] PHP：只读属性
来源：http://hz.cdnleiting.top/gtzgdncosy.html

public readonly string $name
来源：http://hz.jinqigfzy.top/gtutopoujs.html

[U50] PHP：构造器属性提升
来源：http://hz.jinqigfzy.top/gtehkghayd.html

public function __construct(private int $id) {}
来源：http://hz.zhaomingkeji.xyz/gtctpolrip.html


<!-- 参考信息 -->