代发 wailian999

static int counter = 0;
来源：http://hz.ydjk.org.cn/gtngphgebe.html

[S29] C：变参函数
来源：http://hz.ppjwa.cn/gthmcvzlag.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shangyingyoupin.top/gtbjwmvqom.html

[S30] C：头文件保护
来源：http://hz.cashguo.top/gtycwwjhew.html

#ifndef X_H
来源：http://hz.yanxiufei.cn/gtfkbvpmhe.html

#define X_H
来源：http://hz.hysaishi.cn/gtetmzkyoi.html

#endif
来源：http://hz.cdnleiting.top/gtcecbonjs.html

[S31] C++：Hello World
来源：http://hz.yuxming.cn/gtccuofuar.html

#include <iostream>
来源：http://hz.chenzaomai.com/gtxdmnwxmk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuetiantiany.cn/gtdxuhytvm.html

[S32] C++：字符串
来源：http://hz.ydzc1.top/gtrciztzhd.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258.top/gtkzczpcvv.html

[S33] C++：vector 增删
来源：http://hz.yuxming.cn/gtzzpqizyc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sweek.top/gtxpomgkwh.html

[S34] C++：遍历 vector
来源：http://hz.bjfxy.top/gtogtwziwg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ydzc1.top/gtzybzkucm.html

[S35] C++：map
来源：http://hz.pycfn.com/gtgjjghknn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhoulong.xyz/gtbdnmiijc.html

[S36] C++：unordered_map
来源：http://hz.ppjwa.cn/gtsycluuak.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxuanxn.top/gtecwwkycf.html

[S37] C++：set
来源：http://hz.shanyushiyangkeji.top/gtzgspuymr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yj202588.top/gtvmsbeghh.html

[S38] C++：排序
来源：http://hz.hysaishi.cn/gtjcgebyml.html

std::sort(v.begin(), v.end());
来源：http://hz.aizwys.cn/gtznaeihqb.html

[S39] C++：自定义比较器排序
来源：http://hz.jqgufenzy.top/gtnpvlozsi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhoulong.xyz/gthvzvqmno.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangtech.top/gtxbuqtjfp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gzhubu.top/gtwymggfea.html

[S41] C++：类与构造函数
来源：http://hz.yanxiufei.cn/gtdrqukiqu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hnxiangtu.top/gtckhtxiuy.html

[S42] C++：继承与虚函数
来源：http://hz.shangyingyoupin.top/gtvphnbxnv.html

class B : public Base { public: void f() override {} };
来源：http://hz.yangfankeji.com/gtlzxjjexq.html

[S43] C++：智能指针
来源：http://hz.guannengcc.top/gtzcgguafy.html

auto p = std::make_unique<int>(5);
来源：http://hz.feifeiyinyue.top/gtjyxfusmg.html

[S44] C++：引用传参
来源：http://hz.aizwys.cn/gttoxpvqzc.html

void inc(int &x) { ++x; }
来源：http://hz.zhoulong.xyz/gtreavkwwo.html

[S45] C++：lambda
来源：http://hz.xziqi.cn/gtthbmsnpq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aibaodan.cn/gtuwgaruop.html

[S46] C++：函数模板
来源：http://hz.hfpthk.cn/gtdvcqzeom.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cashguo.top/gtxlljyvyt.html

[S47] C++：结构化绑定遍历
来源：http://hz.yanxiufei.cn/gttqhonmce.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.andypj.xyz/gtamdqvfpg.html

[S48] C++：逐行读文件
来源：http://hz.snrcjt.cn/gttjmkacsx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.svipenyu.cn/gtfzkpbdks.html

while (std::getline(in, line)) { }
来源：http://hz.jiagoushi.top/gtrstcsrrk.html

[S49] C++：写文件
来源：http://hz.vqdsnc.cn/gtinbgcvwc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.pengpengdd.cyou/gthcapxfah.html

[S50] C++：格式化数字
来源：http://hz.jqgufenzy.top/gtauqcncsi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yonumen.top/gtvgivszsa.html

[S51] C++：显式类型转换
来源：http://hz.yj202588.top/gtvtapekkc.html

static_cast<double>(a) / b
来源：http://hz.aizwys.cn/gtjqxynxsn.html

[S52] C++：const 与 noexcept
来源：http://hz.sufxvd.cn/gtmdhdyrpe.html

int size() const noexcept { return n_; }
来源：http://hz.cucudq.cn/gtawazpass.html

[S53] C++：移动语义
来源：http://hz.yueranfly.top/gtqvpandqq.html

std::vector<int> w = std::move(v);
来源：http://hz.sysykeji.top/gtxtlucnbe.html

[S54] C++：异常处理
来源：http://hz.snrcjt.cn/gtnijpcqbt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgfzy.top/gtnctuzrxj.html

[S55] C++：结构化绑定
来源：http://hz.daria6918.cn/gtsfinwijy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tanke756.top/gtrdbkcmgh.html

[S56] C++：optional
来源：http://hz.sxryk.cn/gttquxhrbk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj20258888.top/gtbsfofgsq.html

[S57] C++：编译期常量
来源：http://hz.daxiang520.top/gtjdcqvweh.html

constexpr int N = 10;
来源：http://hz.jinqigfzy.top/gtgqawqblt.html

[S58] C++：命名空间
来源：http://hz.9152youxi.cn/gtvtqstslq.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtloeicfhb.html

[S59] C++：静态断言
来源：http://hz.sufxvd.cn/gtduouucxy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.vqdsnc.cn/gtxnmtujyu.html

[S60] C++：遍历并删除元素
来源：http://hz.svipenyu.cn/gtkowglurk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hywenlv.cn/gtrkvkcgcf.html

================================================================================
来源：http://hz.yvedp.cn/gtsopvzypp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daxiang520.top/gtkkxfbzae.html

================================================================================
来源：http://hz.shuidangran.top/gthhgbuxxn.html

[T01] Kotlin：Hello World
来源：http://hz.dianchejie.cn/gtgzmjxghu.html

println("Hello")
来源：http://hz.xinyue.icu/gtxahiwzde.html

[T02] Kotlin：变量
来源：http://hz.vqdsnc.cn/gtaerxmjrk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yonumen.top/gtexwytypa.html

[T03] Kotlin：字符串模板
来源：http://hz.yonumen.top/gtjkygjenl.html

"值: $b"
来源：http://hz.snrcjt.cn/gtdsfyonlw.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangkeji.top/gtgrfqazxh.html

val n: String? = null;  n?.length
来源：http://hz.zhongyouzk.top/gtmzioloax.html

[T05] Kotlin：when 表达式
来源：http://hz.zhengqikj.top/gtwspnwifl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenlongwang.top/gtcfmrowes.html

[T06] Kotlin：集合映射
来源：http://hz.9152youxi.cn/gtjpjvnrts.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinyuanbaomall.cn/gtvqwtzddf.html

[T07] Kotlin：集合过滤
来源：http://hz.9152youxi.cn/gtpmzsgvps.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yangfankeji.com/gtroshhsll.html

[T08] Kotlin：数据类
来源：http://hz.xylfe.cn/gthnvcwfwc.html

data class User(val name: String, val age: Int)
来源：http://hz.feifeiyinyue.top/gttbwazzjp.html

[T09] Kotlin：扩展函数
来源：http://hz.ywan-chungtsiang.top/gtarsvosol.html

fun String.exclaim() = this + "!"
来源：http://hz.jinqigfzy.top/gtftvukyap.html

[T10] Kotlin：默认参数
来源：http://hz.chenjidiqi.icu/gtwpqkpizg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ydzc1.top/gtszbmpyjb.html

[T11] Kotlin：协程
来源：http://hz.hywenlv.cn/gtfcyzjymt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.guannengcc.top/gtsqhilkda.html

[T12] Kotlin：解构声明
来源：http://hz.hammf.cn/gtktdxrory.html

val (a, b) = Pair(1, 2)
来源：http://hz.meibo888.top/gtvzzikwde.html

[T13] Kotlin：只读 Map
来源：http://hz.fengsongda.top/gturfyctkr.html

val m = mapOf("a" to 1)
来源：http://hz.bjfxy.top/gtfzocipis.html

[T14] Kotlin：循环
来源：http://hz.birdmap.top/gtydrecpgw.html

for (i in 1..10) println(i)
来源：http://hz.hysaishi.cn/gtfpitgzzl.html

[T15] Kotlin：接口
来源：http://hz.bjfxy.top/gtsflhnxir.html

interface Shape { fun area(): Double }
来源：http://hz.haohaochexian.top/gtatkthynx.html

[T16] Swift：Hello World
来源：http://hz.gaohongyu789.top/gttsqbyhvt.html

print("Hello")
来源：http://hz.snrcjt.cn/gtowpqqouw.html

[T17] Swift：变量与常量
来源：http://hz.guowangkeji.top/gtdvjbazgd.html

var a = 1;  let b = 2
来源：http://hz.jinyuanbaomall.cn/gtthkknwrj.html

[T18] Swift：字符串插值
来源：http://hz.yvedp.cn/gtxapzvnjb.html

"值: \(b)"
来源：http://hz.feifeiyinyue.top/gtuotebpat.html

[T19] Swift：可选绑定
来源：http://hz.guowangkeji.top/gtoslbquhq.html

if let n = opt { print(n) }
来源：http://hz.yj20258888.top/gtxmcpchoy.html

[T20] Swift：数组操作
来源：http://hz.c1oappe.top/gtclfhcpir.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.quarkkingdee.top/gtrtabcfwp.html

[T21] Swift：遍历
来源：http://hz.bjfxy.top/gthjvpehtk.html

for x in a { print(x) }
来源：http://hz.nanxuanxn.top/gttchxeqpr.html

[T22] Swift：字典
来源：http://hz.svipenyu.cn/gtualfheci.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hammf.cn/gtrgrcnztu.html

[T23] Swift：函数
来源：http://hz.zhoulong.xyz/gthqoiikid.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hysaishi.cn/gtevzvgauo.html

[T24] Swift：闭包
来源：http://hz.hywenlv.cn/gtpklrsbsa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhengqikj.top/gtudagxmrw.html

[T25] Swift：结构体
来源：http://hz.hnxiangtu.top/gtfgzfpdws.html

struct P { var x: Int }
来源：http://hz.fzhhl.top/gtzekuuyyn.html

[T26] Swift：类与重写
来源：http://hz.nwbrower.top/gtjfetjxhh.html

class A: Base { override func f() {} }
来源：http://hz.hongshengwenyu.top/gtbsptuerp.html

[T27] Swift：错误处理
来源：http://hz.zycfv.cn/gtiekjhxxf.html

do { try f() } catch { print(error) }
来源：http://hz.yvedp.cn/gtefspzuhb.html

[T28] Swift：枚举
来源：http://hz.tanke756.top/gtnuviqqba.html

enum Color { case red, green }
来源：http://hz.xuanzx.com/gtwaghoxhh.html

[T29] Swift：guard 提前返回
来源：http://hz.316326.xyz/gtirtgdwcr.html

guard let x = opt else { return }
来源：http://hz.ppjwa.cn/gtdzbfyzhk.html

[T30] Swift：协议
来源：http://hz.hnqzz.top/gtrmjthjbg.html

protocol Shape { func area() -> Double }
来源：http://hz.quarkkingdee.top/gtesnvfkvt.html

[T31] Lua：Hello World
来源：http://hz.wangdashe.top/gtqautbyps.html

print("Hello")
来源：http://hz.svipenyu.cn/gtvbmrtghj.html

[T32] Lua：局部变量
来源：http://hz.hfpthk.cn/gtrmylsodk.html

local a = 1
来源：http://hz.zhixingplan.top/gtpswcnkpx.html

[T33] Lua：表（数组）
来源：http://hz.pycfn.com/gtlrgbfyza.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jqgufenzy.top/gtdnxaehig.html

[T34] Lua：遍历表
来源：http://hz.c1oappe.top/gtnwycefdb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tian-w.cn/gtkjuvkzjp.html

[T35] Lua：字典表
来源：http://hz.jianghu66.top/gtwmmrmfrt.html

local d = { a = 1 };  d.b = 2
来源：http://hz.wangshuangyany.cn/gtqdngyxha.html

[T36] Lua：函数
来源：http://hz.vqdsnc.cn/gtsuwnwymp.html

function add(a, b) return a + b end
来源：http://hz.guowangkeji.top/gtwtjlqdet.html

[T37] Lua：字符串拼接
来源：http://hz.pycfn.com/gtfxrtlhpk.html

"a" .. "b"
来源：http://hz.jinyuanbaomall.cn/gtfkvpuxtn.html

[T38] Lua：条件
来源：http://hz.hammf.cn/gthrlttpyx.html

if x > 0 then print("正") end
来源：http://hz.sweek.top/gtvuxuwsto.html

[T39] Lua：模式匹配
来源：http://hz.yuanzhike.top/gtucypywhp.html

string.find(s, "%d+")
来源：http://hz.sxryk.cn/gthsnfjrro.html

[T40] Lua：元表
来源：http://hz.guowangkeji.top/gtncxcuact.html

setmetatable({}, { __index = base })
来源：http://hz.yonumen.top/gtzwvxuexx.html

[T41] Perl：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtufxkdisy.html

print "Hello\n";
来源：http://hz.zhiwuduotai.top/gtudoyslnd.html

[T42] Perl：变量类型
来源：http://hz.hfpthk.cn/gtvvhfifyn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.havefunace.top/gtbubgagaa.html

[T43] Perl：字符串插值
来源：http://hz.aizwys.cn/gtdpdfuvuc.html

"值: $a"
来源：http://hz.zycfv.cn/gthhvligix.html

[T44] Perl：条件
来源：http://hz.zhengqikj.top/gtgyvpmhos.html

if ($a > 0) { print "正"; }
来源：http://hz.9152youxi.cn/gtwqaselkc.html

[T45] Perl：数组遍历
来源：http://hz.ppjwa.cn/gtekhyocqu.html

for my $x (@arr) { print $x; }
来源：http://hz.zycfv.cn/gtgpbkcdpl.html

[T46] Perl：哈希操作
来源：http://hz.jlsjyb.cn/gtmaozszxh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shuidangran.top/gtejwhpmrq.html

[T47] Perl：正则捕获
来源：http://hz.yonumen.top/gtikofmcam.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xuetiantiany.cn/gtnvxrjhnn.html

[T48] Perl：正则替换
来源：http://hz.yvedp.cn/gtizqvqqxv.html

$s =~ s/old/new/g;
来源：http://hz.316326.xyz/gtymsmfcya.html

[T49] Perl：函数
来源：http://hz.jinyuanbaomall.cn/gtrfsgemvi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtzjhswwpt.html

[T50] Perl：逐行读文件
来源：http://hz.mhx1999.top/gtjrfhazsg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hammf.cn/gtemopvzye.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.andypj.xyz/gtzbxzkqym.html

[T51] Scala：Hello World
来源：http://hz.shanyushiyangkeji.top/gtyttdtalu.html

println("Hello")
来源：http://hz.yvedp.cn/gtcfgcordo.html

[T52] Scala：变量
来源：http://hz.zhixingplan.top/gtasizcmye.html

val a = 1;  var b = 2
来源：http://hz.0kj1m.cn/gtiqbrdjyn.html

[T53] Scala：字符串插值
来源：http://hz.jinqigfzy.top/gtccglfrly.html

s"值: $b"
来源：http://hz.hnqzz.top/gtlhfvdhca.html

[T54] Scala：集合映射
来源：http://hz.wangdashe.top/gtnbwsotbp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yueranfly.top/gtoqchakto.html

[T55] Scala：集合过滤
来源：http://hz.zhaomingkeji.xyz/gtdxrbljir.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.meibo888.top/gtdtrooocw.html

[T56] Scala：样例类
来源：http://hz.yvedp.cn/gtowoenwlx.html

case class User(name: String, age: Int)
来源：http://hz.ydzc1.top/gtrhfyacvh.html

[T57] Scala：模式匹配
来源：http://hz.xingfuxueyuan.xyz/gthysozdcs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xingfuxueyuan.xyz/gtcgeeluyn.html

[T58] Scala：函数定义
来源：http://hz.shzxlz.cn/gthcqyxkzx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ybcxt.top/gtekydwukh.html

[T59] Scala：循环
来源：http://hz.c1oappe.top/gtaclabdep.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenlongwang.top/gtmfuvpfqa.html

[T60] Scala：折叠
来源：http://hz.jinqigufen.top/gtigxzzuer.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jianghu66.top/gtsxkeumlp.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtabjtimnn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhoulong.xyz/gthotzmqqf.html

================================================================================
来源：http://hz.gotoacloud.top/gtmaqnctff.html

[U01] Py：创建虚拟环境
来源：http://hz.smart0.xyz/gtdgtgspbs.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhixingplan.top/gtabcelvey.html

[U02] Py：导出 / 安装依赖
来源：http://hz.quarkkingdee.top/gtyyyuzjsy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.snrcjt.cn/gtwfxhtyul.html

[U03] Py：加载 .env 配置
来源：http://hz.tian-w.cn/gtxnjprhmq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.cashguo.top/gtopshnpmc.html

[U04] Py：变量调试打印
来源：http://hz.jinyuanbaomall.cn/gttckqxbtm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258888.top/gtdbvphjle.html

[U05] Py：列表去重且保序
来源：http://hz.fengsongda.top/gtvgenwmev.html

list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtjdnmnphf.html

[U06] Py：合并两个字典
来源：http://hz.xuanzx.com/gtqtfquetm.html

{**a, **b}
来源：http://hz.haohaochexian.top/gtznnidldm.html

[U07] Py：反转字典键值
来源：http://hz.jinqigufen.top/gtmjcomcgx.html

{v: k for k, v in d.items()}
来源：http://hz.cqqwz.cn/gtlfvritna.html

[U08] Py：展平二维列表
来源：http://hz.zhengqikj.top/gtmibeomfz.html

[y for x in nested for y in x]
来源：http://hz.jianghu66.top/gtbzudumzj.html

[U09] Py：字典取最大值的键
来源：http://hz.nwbrower.top/gtdayjoovp.html

max(d, key=d.get)
来源：http://hz.sysykeji.top/gtdmzwzgae.html

[U10] Py：按值排序字典
来源：http://hz.fzhhl.top/gtvlczujzc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yj20258.top/gtwjluayyx.html

[U11] Py：生成器表达式
来源：http://hz.nwbrower.top/gtgntejjzl.html

(x * 2 for x in arr)
来源：http://hz.ybcxt.top/gthdptmwrd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.pycfn.com/gtzcgcenfj.html

Counter(arr).most_common(3)
来源：http://hz.hongshengwenyu.top/gtmucetimy.html

[U13] Py：固定长度队列
来源：http://hz.jinyuanbaomall.cn/gtbnwglfph.html

deque(maxlen=10)
来源：http://hz.jiagoushi.top/gtcxitqomy.html

[U14] Py：分组收集到列表
来源：http://hz.chenjidiqi.icu/gteqtrfcju.html

defaultdict(list)
来源：http://hz.hywenlv.cn/gtxryrerpn.html

[U15] Py：高精度计时
来源：http://hz.aizwys.cn/gtyjxkfkcw.html

t = time.perf_counter()
来源：http://hz.fengsongda.top/gtpdkokesu.html

[U16] Py：命令行参数解析
来源：http://hz.tanke756.top/gtsrqilogj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hammf.cn/gtlscyjjqo.html

[U17] Py：初始化日志
来源：http://hz.cheryme.top/gtcpsopxnf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xingfuxueyuan.xyz/gtjmhjryoz.html

[U18] Py：预编译正则
来源：http://hz.zhiwuduotai.top/gtaiotupgq.html

pat = re.compile(r"\d+")
来源：http://hz.yj20258.top/gtzqrpqggb.html

[U19] Py：正则替换带回调
来源：http://hz.jinqigufen.top/gtfocoptxb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.nanxinkj.top/gtjylhuowp.html

[U20] Py：缓存函数结果
来源：http://hz.jqgfzy.top/gtedainjtx.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shuidangran.top/gtnqnrtbkw.html

[U21] Py：自定义上下文管理器
来源：http://hz.hywenlv.cn/gthlnmehsx.html

@contextlib.contextmanager
来源：http://hz.birdmap.top/gtzqiinesj.html

[U22] Py：矩阵转置
来源：http://hz.aibaodan.cn/gtmehkwdxd.html

list(zip(*m))
来源：http://hz.hongshengwenyu.top/gtorhpoujp.html

[U23] Py：分块读取大文件
来源：http://hz.fengsongda.top/gtylcotgsp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sufxvd.cn/gtrbaqdklv.html

[U24] Py：路径操作
来源：http://hz.smart0.xyz/gtgieplobp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shanyushiyangkeji.top/gtwqncmovt.html

[U25] Py：CSV 按字典读
来源：http://hz.gaohongyu789.top/gtrnzcasqh.html

csv.DictReader(f)
来源：http://hz.cqqwz.cn/gtntlajfsq.html

[U26] Py：并发下载
来源：http://hz.birdmap.top/gtaxzmltbh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhongyouzk.top/gtnmoadsew.html

[U27] Py：异步 HTTP
来源：http://hz.zhiwuduotai.top/gtoqwigiff.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yueranfly.top/gtggobmarv.html

[U28] Py：类型别名
来源：http://hz.meibo888.top/gtrsfzvlwv.html

UserId = int
来源：http://hz.chenjidiqi.icu/gtmpizmzcj.html

[U29] Py：属性校验
来源：http://hz.0kj1m.cn/gtihnrxalx.html

@property 与 @x.setter 配合
来源：http://hz.shangyingyoupin.top/gteivwaivc.html

[U30] Py：数据类
来源：http://hz.jiagoushi.top/gtnrakqdgs.html

@dataclass(slots=True)
来源：http://hz.yj20258888.top/gtjvnrfiwe.html

[U31] Py：单测
来源：http://hz.nanxinkj.top/gtgopkknxh.html

python -m pytest -q
来源：http://hz.chenzaomai.com/gtarxguhjm.html

[U32] Py：代码格式化
来源：http://hz.xuanzx.com/gtpbedbsqn.html

ruff format . && ruff check --fix .
来源：http://hz.mhx1999.top/gtbvqcgxoe.html

[U33] Py：打包发布
来源：http://hz.316326.xyz/gtihsmjblt.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.feifeiyinyue.top/gtpbgsdvuq.html

[U34] Py：判断编码
来源：http://hz.xinyue.icu/gtwdwohkoq.html

chardet.detect(raw)
来源：http://hz.xuanzx.com/gtyrssvcxp.html

[U35] Py：发送邮件
来源：http://hz.zhaomingkeji.xyz/gtzjptjroq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.chenjidiqi.icu/gtotfjexqr.html

[U36] Py：定时任务
来源：http://hz.ydjk.org.cn/gtizctbzwi.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhijiandao.cn/gtnxnocpxd.html

[U37] Py：读写 Excel
来源：http://hz.tian-w.cn/gtkxwnpdkr.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hnxiangtu.top/gthmcncrrd.html

[U38] Py：获取脚本所在目录
来源：http://hz.birdmap.top/gtienyitbo.html

Path(__file__).resolve().parent
来源：http://hz.52xcode.cn/gteyelosci.html

[U39] Py：判断是否在交互环境
来源：http://hz.birdmap.top/gtmwcictil.html

sys.stdout.isatty()
来源：http://hz.xingfuxueyuan.xyz/gttnfhdqva.html

[U40] Py：打印到标准错误
来源：http://hz.snrcjt.cn/gtjxnbaixc.html

print("err", file=sys.stderr)
来源：http://hz.ydjk.org.cn/gtooqrucfy.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hysaishi.cn/gtgvvzoofu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hongshengwenyu.top/gtqfaykjiv.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.fzhhl.top/gtzrnklara.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jlsjyb.cn/gtvqhhqxpu.html

[U43] PHP：声明命名空间
来源：http://hz.yvedp.cn/gtlszbtfhs.html

namespace App\Http;
来源：http://hz.redwolf501.top/gtfnrmdpbg.html

[U44] PHP：开启严格类型
来源：http://hz.jinqigfzy.top/gtbsdssrfz.html

declare(strict_types=1);
来源：http://hz.havefunace.top/gthyhigmwl.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jinyuanbaomall.cn/gtajsjxdnj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtohldhofd.html

[U46] PHP：可空类型
来源：http://hz.vqdsnc.cn/gtdtsauyln.html

?string $name = null
来源：http://hz.hywenlv.cn/gtpnkicfui.html

[U47] PHP：联合类型
来源：http://hz.xingfuxueyuan.xyz/gtgqgusizp.html

int|string $id
来源：http://hz.jinghuilouyu.cn/gtfrkulybk.html

[U48] PHP：纯枚举
来源：http://hz.dianchejie.cn/gtomwptydv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yvedp.cn/gtetxbchuc.html

[U49] PHP：只读属性
来源：http://hz.ywan-chungtsiang.top/gtajpxtcvk.html

public readonly string $name
来源：http://hz.ivvv.top/gtpjsmljcb.html

[U50] PHP：构造器属性提升
来源：http://hz.yonumen.top/gtlairglbs.html

public function __construct(private int $id) {}
来源：http://hz.yangfankeji.com/gtnlhkayoq.html

[U51] PHP：数组解构
来源：http://hz.cheryme.top/gtfodrkfqr.html

[$a, $b] = $arr;
来源：http://hz.jinyuanbaomall.cn/gtqtwrgqzh.html

[U52] PHP：箭头函数
来源：http://hz.pengpengdd.cyou/gtlchesmxc.html

$double = fn($x) => $x * 2;
来源：http://hz.sweek.top/gtycfxisss.html


<!-- 参考信息 -->