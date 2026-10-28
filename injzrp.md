代发 wailian999

#ifndef X_H
来源：http://hz.xinyue.icu/gtqhzlnbeo.html

#define X_H
来源：http://hz.jianghu66.top/gtchgnbpal.html

#endif
来源：http://hz.xingfuxueyuan.xyz/gtwxkuxume.html

[S31] C++：Hello World
来源：http://hz.nwbrower.top/gtuwblvfcb.html

#include <iostream>
来源：http://hz.ppjwa.cn/gtmzewuwsv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cheryme.top/gtosmdmvbu.html

[S32] C++：字符串
来源：http://hz.ybcxt.top/gtfkjmbrmn.html

std::string s = "hi";  s += "!";
来源：http://hz.tian-w.cn/gthguzbxmm.html

[S33] C++：vector 增删
来源：http://hz.nanxinkj.top/gtvhsujnal.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxinkj.top/gtyobfokmk.html

[S34] C++：遍历 vector
来源：http://hz.jlsjyb.cn/gtxmamrpha.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.havefunace.top/gtxuuhzppi.html

[S35] C++：map
来源：http://hz.dianchejie.cn/gtpdzscypv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuxming.cn/gtcqagvydy.html

[S36] C++：unordered_map
来源：http://hz.mhx1999.top/gtirexwzao.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.0kj1m.cn/gtlbuighzx.html

[S37] C++：set
来源：http://hz.zhixingplan.top/gtucasekeb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hfpthk.cn/gtzsucaewh.html

[S38] C++：排序
来源：http://hz.jianghu66.top/gtpczpmisx.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gthowwfjyz.html

[S39] C++：自定义比较器排序
来源：http://hz.cashguo.top/gtmdawooke.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnxiangtu.top/gtupwtqsvx.html

[S40] C++：查找元素
来源：http://hz.zhengqikj.top/gtknebvcvw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhoulong.xyz/gtdpdbcvhk.html

[S41] C++：类与构造函数
来源：http://hz.zhiwuduotai.top/gtmeiedbae.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shanyushiyangkeji.top/gtvxijqlwn.html

[S42] C++：继承与虚函数
来源：http://hz.xuetiantiany.cn/gtkpkxdrwj.html

class B : public Base { public: void f() override {} };
来源：http://hz.ydjk.org.cn/gtshyprtuc.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gtoofxmjed.html

auto p = std::make_unique<int>(5);
来源：http://hz.vqdsnc.cn/gtcpkmqvlg.html

[S44] C++：引用传参
来源：http://hz.zhijiandao.cn/gtvvngwvvd.html

void inc(int &x) { ++x; }
来源：http://hz.cqqwz.cn/gtoaaisrwa.html

[S45] C++：lambda
来源：http://hz.zhixingplan.top/gtfamgiguv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxuanxn.top/gthtgzxrxi.html

[S46] C++：函数模板
来源：http://hz.sxryk.cn/gtqihdbmci.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yonumen.top/gtoejxkjhu.html

[S47] C++：结构化绑定遍历
来源：http://hz.jiagoushi.top/gtprbfauoc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gaohongyu789.top/gtdpmhjzuu.html

[S48] C++：逐行读文件
来源：http://hz.yanxiufei.cn/gtrsheiuyo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.fzhhl.top/gtgbtxxlii.html

while (std::getline(in, line)) { }
来源：http://hz.jyoumei.cn/gtczblwdhj.html

[S49] C++：写文件
来源：http://hz.cheryme.top/gtznwnfoam.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.quarkkingdee.top/gtpzrtglux.html

[S50] C++：格式化数字
来源：http://hz.xinyue.icu/gtnxtrjgrn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.smart0.xyz/gtyqtzaexx.html

[S51] C++：显式类型转换
来源：http://hz.yuxming.cn/gtkgwabpcb.html

static_cast<double>(a) / b
来源：http://hz.dashuyun.cn/gtgqhmgoxj.html

[S52] C++：const 与 noexcept
来源：http://hz.zhongyouzk.top/gtvdqcinam.html

int size() const noexcept { return n_; }
来源：http://hz.yongpay.top/gttakyjgdh.html

[S53] C++：移动语义
来源：http://hz.quarkkingdee.top/gtvdfbaygi.html

std::vector<int> w = std::move(v);
来源：http://hz.birdmap.top/gtoemmlsiu.html

[S54] C++：异常处理
来源：http://hz.0kj1m.cn/gtaajltajd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhengqikj.top/gtnsxexcfk.html

[S55] C++：结构化绑定
来源：http://hz.tanke756.top/gtvfjlgemo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuxming.cn/gtsjzlqnlm.html

[S56] C++：optional
来源：http://hz.gotoacloud.top/gtvglesrhz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tianlin.xyz/gtknvoougv.html

[S57] C++：编译期常量
来源：http://hz.xingfuxueyuan.xyz/gtbxhnzbzs.html

constexpr int N = 10;
来源：http://hz.nanxuanxn.top/gtcfafkcno.html

[S58] C++：命名空间
来源：http://hz.hfpthk.cn/gtzkwizdna.html

namespace ns { int f() { return 1; } }
来源：http://hz.ywan-chungtsiang.top/gtsrkjfazb.html

[S59] C++：静态断言
来源：http://hz.gzhubu.top/gtrzmpfhhb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zycfv.cn/gtlamsvhwq.html

[S60] C++：遍历并删除元素
来源：http://hz.fzhhl.top/gtpfdteogh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.c1oappe.top/gtbugfdnhh.html

================================================================================
来源：http://hz.yuxming.cn/gthydmbepw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhaomingkeji.xyz/gtsmgpwuko.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtbiknzulv.html

[T01] Kotlin：Hello World
来源：http://hz.xuetiantiany.cn/gtxamobnlc.html

println("Hello")
来源：http://hz.daxiang520.top/gtygvidzru.html

[T02] Kotlin：变量
来源：http://hz.pengpengdd.cyou/gtjpwbwnit.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.dianchejie.cn/gtpyzmnmgh.html

[T03] Kotlin：字符串模板
来源：http://hz.yangfankeji.com/gtwzfrbvwc.html

"值: $b"
来源：http://hz.jqgufenzy.top/gtfznqtckx.html

[T04] Kotlin：空安全
来源：http://hz.tanke756.top/gtizzdngxg.html

val n: String? = null;  n?.length
来源：http://hz.guannengcc.top/gtqnqbuofl.html

[T05] Kotlin：when 表达式
来源：http://hz.chenlongwang.top/gtzqyiyssg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.quarkkingdee.top/gtwlhomeww.html

[T06] Kotlin：集合映射
来源：http://hz.hysaishi.cn/gtdzifnoie.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gzhubu.top/gtcizpiddv.html

[T07] Kotlin：集合过滤
来源：http://hz.xylfe.cn/gtrzwlpanr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jyoumei.cn/gtlwhzrpim.html

[T08] Kotlin：数据类
来源：http://hz.yangfankeji.com/gtckakezvk.html

data class User(val name: String, val age: Int)
来源：http://hz.yonumen.top/gtakrrjiyt.html

[T09] Kotlin：扩展函数
来源：http://hz.ehwqpu.com/gtiaogtfbc.html

fun String.exclaim() = this + "!"
来源：http://hz.aibaodan.cn/gtrpmbvfxy.html

[T10] Kotlin：默认参数
来源：http://hz.fengsongda.top/gtjewrkikk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daria6918.cn/gtfbzcndko.html

[T11] Kotlin：协程
来源：http://hz.yvedp.cn/gthaccshvr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jqgfzy.top/gtuimzqdwr.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtuwpkkdhu.html

val (a, b) = Pair(1, 2)
来源：http://hz.snrcjt.cn/gtxmbgsdzz.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258888.top/gtksgercmu.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtaexqifrf.html

[T14] Kotlin：循环
来源：http://hz.jinqigfzy.top/gtojkrukgh.html

for (i in 1..10) println(i)
来源：http://hz.xuetiantiany.cn/gtyywjuery.html

[T15] Kotlin：接口
来源：http://hz.snrcjt.cn/gtxjxjsspu.html

interface Shape { fun area(): Double }
来源：http://hz.chenzaomai.com/gtpvfrgdqd.html

[T16] Swift：Hello World
来源：http://hz.hysaishi.cn/gtfpkdaeuy.html

print("Hello")
来源：http://hz.yueranfly.top/gtuwehyquj.html

[T17] Swift：变量与常量
来源：http://hz.sysykeji.top/gtuejnfgsd.html

var a = 1;  let b = 2
来源：http://hz.jqgufenzy.top/gtumfggfqd.html

[T18] Swift：字符串插值
来源：http://hz.jinqigfzy.top/gtxjwcyeir.html

"值: \(b)"
来源：http://hz.aizwys.cn/gtmhooddbp.html

[T19] Swift：可选绑定
来源：http://hz.0kj1m.cn/gtyvwiqiyf.html

if let n = opt { print(n) }
来源：http://hz.jinqigufen.top/gtlfzdvyrw.html

[T20] Swift：数组操作
来源：http://hz.ivvv.top/gtixzqsxtd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangkeji.top/gtilmjdisu.html

[T21] Swift：遍历
来源：http://hz.nanxuanxn.top/gtpziadajq.html

for x in a { print(x) }
来源：http://hz.yuanzhike.top/gthrwhxgkw.html

[T22] Swift：字典
来源：http://hz.xziqi.cn/gtyfmmixcl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zycfv.cn/gtftjvudrs.html

[T23] Swift：函数
来源：http://hz.52xcode.cn/gtjucpioui.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenjidiqi.icu/gtovehwkiw.html

[T24] Swift：闭包
来源：http://hz.jinqigfzy.top/gtmsicvnux.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hnqzz.top/gtygkucujk.html

[T25] Swift：结构体
来源：http://hz.aizwys.cn/gtycezlqdu.html

struct P { var x: Int }
来源：http://hz.zhixingplan.top/gtgplbxmol.html

[T26] Swift：类与重写
来源：http://hz.jqgfzy.top/gtgnvigntp.html

class A: Base { override func f() {} }
来源：http://hz.jinyuanbaomall.cn/gtuktpvtuj.html

[T27] Swift：错误处理
来源：http://hz.zhoulong.xyz/gtyxzxtgya.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigfzy.top/gtqusipaxp.html

[T28] Swift：枚举
来源：http://hz.ybcxt.top/gtgwzgesdd.html

enum Color { case red, green }
来源：http://hz.hammf.cn/gtmntvjxzw.html

[T29] Swift：guard 提前返回
来源：http://hz.guannengcc.top/gtefcpocso.html

guard let x = opt else { return }
来源：http://hz.nanxuanxn.top/gtbxwbvalf.html

[T30] Swift：协议
来源：http://hz.jinyuanbaomall.cn/gtkwyoimmx.html

protocol Shape { func area() -> Double }
来源：http://hz.zhongyouzk.top/gtadqhrkgo.html

[T31] Lua：Hello World
来源：http://hz.yj20258888.top/gtqvztdopp.html

print("Hello")
来源：http://hz.ywan-chungtsiang.top/gtwfvgfvup.html

[T32] Lua：局部变量
来源：http://hz.yanxiufei.cn/gtqeudltty.html

local a = 1
来源：http://hz.dianchejie.cn/gtsyfmsgvk.html

[T33] Lua：表（数组）
来源：http://hz.hnxiangtu.top/gtkygqwedq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.chenjidiqi.icu/gtpgswxnrv.html

[T34] Lua：遍历表
来源：http://hz.0kj1m.cn/gtyiayraeq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ywan-chungtsiang.top/gtvwhhmkij.html

[T35] Lua：字典表
来源：http://hz.ydzc1.top/gtjbbbdnaq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jianghu66.top/gtdtvitsvt.html

[T36] Lua：函数
来源：http://hz.quarkkingdee.top/gtwqybuslo.html

function add(a, b) return a + b end
来源：http://hz.nanxuanxn.top/gtxinkjzbt.html

[T37] Lua：字符串拼接
来源：http://hz.ehwqpu.com/gtewojskpe.html

"a" .. "b"
来源：http://hz.xinyue.icu/gtzsxuiehf.html

[T38] Lua：条件
来源：http://hz.cdnleiting.top/gtqcerlyso.html

if x > 0 then print("正") end
来源：http://hz.jlsjyb.cn/gtdajtucdd.html

[T39] Lua：模式匹配
来源：http://hz.dashuyun.cn/gtssnhdkui.html

string.find(s, "%d+")
来源：http://hz.kuanghao11.cn/gtrjsonzbq.html

[T40] Lua：元表
来源：http://hz.fengsongda.top/gtxehfhtsc.html

setmetatable({}, { __index = base })
来源：http://hz.zdqjudy.top/gthdtrgbcx.html

[T41] Perl：Hello World
来源：http://hz.zhixingplan.top/gtpransgaa.html

print "Hello\n";
来源：http://hz.yuxming.cn/gtqfypznrb.html

[T42] Perl：变量类型
来源：http://hz.52xcode.cn/gtwkpnyvfo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sxryk.cn/gtriacmtkx.html

[T43] Perl：字符串插值
来源：http://hz.snrcjt.cn/gtqkvintzr.html

"值: $a"
来源：http://hz.fzhhl.top/gthizvvdhd.html

[T44] Perl：条件
来源：http://hz.shanyushiyangtech.top/gtujjiclqh.html

if ($a > 0) { print "正"; }
来源：http://hz.316326.xyz/gtfaiwhcpd.html

[T45] Perl：数组遍历
来源：http://hz.shangyingyoupin.top/gtcqqbjcoq.html

for my $x (@arr) { print $x; }
来源：http://hz.hfpthk.cn/gtwsijmewv.html

[T46] Perl：哈希操作
来源：http://hz.9152youxi.cn/gtechitdtk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yonumen.top/gtzppwedoe.html

[T47] Perl：正则捕获
来源：http://hz.zhiwuduotai.top/gtnjjikwzr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.aibaodan.cn/gttoadqchh.html

[T48] Perl：正则替换
来源：http://hz.yonumen.top/gtxsigklyg.html

$s =~ s/old/new/g;
来源：http://hz.yanxiufei.cn/gtqbmoyadw.html

[T49] Perl：函数
来源：http://hz.mhx1999.top/gtfkvzbifn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hnqzz.top/gtzllgbsff.html

[T50] Perl：逐行读文件
来源：http://hz.cucudq.cn/gtsziglnos.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.meibo888.top/gtppfwkyfk.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yanxiufei.cn/gthzqrywdt.html

[T51] Scala：Hello World
来源：http://hz.yueranfly.top/gtihscuyea.html

println("Hello")
来源：http://hz.52xcode.cn/gtngazvxgf.html

[T52] Scala：变量
来源：http://hz.iojbl.cn/gtahrvzlxd.html

val a = 1;  var b = 2
来源：http://hz.c1oappe.top/gtnqlgmipb.html

[T53] Scala：字符串插值
来源：http://hz.jyoumei.cn/gtgroeplmt.html

s"值: $b"
来源：http://hz.hnxiangtu.top/gtjvabctin.html

[T54] Scala：集合映射
来源：http://hz.yuanzhike.top/gtxyzccdbq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hongshengwenyu.top/gtqtjtlgzt.html

[T55] Scala：集合过滤
来源：http://hz.aibaodan.cn/gtpyzfvgmw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.wangshuangyany.cn/gtobmidyuj.html

[T56] Scala：样例类
来源：http://hz.dianchejie.cn/gtjcnfemdu.html

case class User(name: String, age: Int)
来源：http://hz.shuidangran.top/gtblugunfb.html

[T57] Scala：模式匹配
来源：http://hz.wangdashe.top/gtmiezpbpg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.tian-w.cn/gtzyvxeice.html

[T58] Scala：函数定义
来源：http://hz.hammf.cn/gtrqwgozow.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.mhx1999.top/gtamjkjdyw.html

[T59] Scala：循环
来源：http://hz.shanyushiyangkeji.top/gtauyxoywi.html

for (i <- 1 to 10) println(i)
来源：http://hz.jqgufenzy.top/gtjinigcsm.html

[T60] Scala：折叠
来源：http://hz.yj20258888.top/gtenhekvqz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.mhx1999.top/gtrbheknbh.html

================================================================================
来源：http://hz.cashguo.top/gtcgpbaapc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.fengsongda.top/gtuiujjfzr.html

================================================================================
来源：http://hz.fengsongda.top/gtjohwivqd.html

[U01] Py：创建虚拟环境
来源：http://hz.zhiwuduotai.top/gtktiguvpx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ppjwa.cn/gtcpgdsfjt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shzxlz.cn/gtkfpgrchf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zycfv.cn/gtlcdzqkat.html

[U03] Py：加载 .env 配置
来源：http://hz.shzxlz.cn/gtcpmhbkpu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhengqikj.top/gtjaftujus.html

[U04] Py：变量调试打印
来源：http://hz.pengpengdd.cyou/gtpueghzwq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tanke756.top/gtedwbfjik.html

[U05] Py：列表去重且保序
来源：http://hz.shanyushiyangtech.top/gtcnbzrmwh.html

list(dict.fromkeys(arr))
来源：http://hz.snrcjt.cn/gtadyfeffh.html

[U06] Py：合并两个字典
来源：http://hz.yongpay.top/gtstseyevn.html

{**a, **b}
来源：http://hz.jinghuilouyu.cn/gtqatddjhu.html

[U07] Py：反转字典键值
来源：http://hz.chenlongwang.top/gtmtmaxtda.html

{v: k for k, v in d.items()}
来源：http://hz.jqgufenzy.top/gtjzqcaesh.html

[U08] Py：展平二维列表
来源：http://hz.jinqigfzy.top/gtyguwroma.html

[y for x in nested for y in x]
来源：http://hz.guannengcc.top/gtvwwarnpa.html

[U09] Py：字典取最大值的键
来源：http://hz.smart0.xyz/gthkadrufw.html

max(d, key=d.get)
来源：http://hz.52xcode.cn/gtpbcbwywr.html

[U10] Py：按值排序字典
来源：http://hz.ybcxt.top/gtdddtaenz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xuetiantiany.cn/gtqpgxyvcb.html

[U11] Py：生成器表达式
来源：http://hz.sxryk.cn/gtjqfhhiqk.html

(x * 2 for x in arr)
来源：http://hz.guowangkeji.top/gtedzbxhtb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.guannengcc.top/gtcqgstdjr.html

Counter(arr).most_common(3)
来源：http://hz.yj202588.top/gtqkauisyw.html

[U13] Py：固定长度队列
来源：http://hz.zycfv.cn/gtyigszzfe.html

deque(maxlen=10)
来源：http://hz.yonumen.top/gthimptfzo.html

[U14] Py：分组收集到列表
来源：http://hz.xingfuxueyuan.xyz/gtfifgndpq.html

defaultdict(list)
来源：http://hz.zycfv.cn/gtwplbbyme.html

[U15] Py：高精度计时
来源：http://hz.daxiang520.top/gterrfdfkk.html

t = time.perf_counter()
来源：http://hz.jqgfzy.top/gtmqxbvxyx.html

[U16] Py：命令行参数解析
来源：http://hz.jinqigufen.top/gtsihctvkf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gzhubu.top/gtrbeyucle.html

[U17] Py：初始化日志
来源：http://hz.redwolf501.top/gttxpogmmg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ydjk.org.cn/gtfsxcyawh.html

[U18] Py：预编译正则
来源：http://hz.meibo888.top/gtoxfjpnks.html

pat = re.compile(r"\d+")
来源：http://hz.ywan-chungtsiang.top/gtdzdsnqqr.html

[U19] Py：正则替换带回调
来源：http://hz.zycfv.cn/gtdukbtflf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.snrcjt.cn/gtsawyscit.html

[U20] Py：缓存函数结果
来源：http://hz.ywan-chungtsiang.top/gtxtlvjlqw.html

@functools.lru_cache(maxsize=None)
来源：http://hz.cqqwz.cn/gtbntzrszs.html

[U21] Py：自定义上下文管理器
来源：http://hz.yueranfly.top/gtkzbuxmvz.html

@contextlib.contextmanager
来源：http://hz.ybcxt.top/gtrcrsvpyn.html

[U22] Py：矩阵转置
来源：http://hz.ybcxt.top/gtvckabcuo.html

list(zip(*m))
来源：http://hz.yuxming.cn/gtbekelybt.html

[U23] Py：分块读取大文件
来源：http://hz.chenzaomai.com/gthsrbuwzt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.kuanghao11.cn/gtbhdhhpkx.html

[U24] Py：路径操作
来源：http://hz.haohaochexian.top/gtpxhwcqjf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cheryme.top/gtevowvnlh.html

[U25] Py：CSV 按字典读
来源：http://hz.yangfankeji.com/gtwzituvhx.html

csv.DictReader(f)
来源：http://hz.fzhhl.top/gtjwuepzwg.html

[U26] Py：并发下载
来源：http://hz.shzxlz.cn/gtohkgykwc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.havefunace.top/gtlyptegfq.html

[U27] Py：异步 HTTP
来源：http://hz.aibaodan.cn/gtmopbyifl.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hfpthk.cn/gtabvzvpcx.html

[U28] Py：类型别名
来源：http://hz.birdmap.top/gtiwkpoucv.html

UserId = int
来源：http://hz.feifeiyinyue.top/gtbcysfygf.html

[U29] Py：属性校验
来源：http://hz.cheryme.top/gtwfyzpkhw.html

@property 与 @x.setter 配合
来源：http://hz.guannengcc.top/gtciwprqnl.html

[U30] Py：数据类
来源：http://hz.fzhhl.top/gteiafgmqn.html

@dataclass(slots=True)
来源：http://hz.ybcxt.top/gtygkvcncc.html

[U31] Py：单测
来源：http://hz.ivvv.top/gtdmybrzsx.html

python -m pytest -q
来源：http://hz.yueranfly.top/gtpwudejjj.html

[U32] Py：代码格式化
来源：http://hz.xingfuxueyuan.xyz/gtdjdxkknw.html

ruff format . && ruff check --fix .
来源：http://hz.daxiang520.top/gtfnhychkp.html

[U33] Py：打包发布
来源：http://hz.gzhubu.top/gtiaprdlfd.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ydzc1.top/gtviplvuet.html

[U34] Py：判断编码
来源：http://hz.zycfv.cn/gtkwjnairt.html

chardet.detect(raw)
来源：http://hz.havefunace.top/gtyduckkoc.html

[U35] Py：发送邮件
来源：http://hz.zycfv.cn/gtgcafsjxj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zycfv.cn/gtsavgexat.html

[U36] Py：定时任务
来源：http://hz.smart0.xyz/gtdlejemcw.html

schedule.every(10).minutes.do(job)
来源：http://hz.hnqzz.top/gtdensguow.html

[U37] Py：读写 Excel
来源：http://hz.sweek.top/gtcspezueh.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yuanzhike.top/gtgpowotpm.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhijiandao.cn/gtrnxtvvwv.html

Path(__file__).resolve().parent
来源：http://hz.jinyuanbaomall.cn/gtmoavczxh.html

[U39] Py：判断是否在交互环境
来源：http://hz.hongshengwenyu.top/gtlvckvtot.html

sys.stdout.isatty()
来源：http://hz.jinyuanbaomall.cn/gtzpjxctun.html

[U40] Py：打印到标准错误
来源：http://hz.ybcxt.top/gteealdrna.html

print("err", file=sys.stderr)
来源：http://hz.chenjidiqi.icu/gtxblbgyzq.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenzaomai.com/gtrxudgpkv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hnqzz.top/gtodcexkli.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yj20258.top/gtmcjvpvya.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.sweek.top/gtisdubnxi.html

[U43] PHP：声明命名空间
来源：http://hz.quarkkingdee.top/gtldvrvgeb.html

namespace App\Http;
来源：http://hz.shanyushiyangtech.top/gtohhflvui.html

[U44] PHP：开启严格类型
来源：http://hz.dianchejie.cn/gtkjzrrlhm.html

declare(strict_types=1);
来源：http://hz.yj202588.top/gttkjoxubr.html

[U45] PHP：类型声明与返回类型
来源：http://hz.0kj1m.cn/gtifvzvgvz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yanxiufei.cn/gtrmnjdlur.html

[U46] PHP：可空类型
来源：http://hz.jianghu66.top/gtvpqhvzba.html

?string $name = null
来源：http://hz.yj202588.top/gtsbopamkb.html

[U47] PHP：联合类型
来源：http://hz.haohaochexian.top/gtzbtdztud.html

int|string $id
来源：http://hz.316326.xyz/gtybmjeokg.html

[U48] PHP：纯枚举
来源：http://hz.chenlongwang.top/gtsewukgyw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinyuanbaomall.cn/gtckriacbr.html

[U49] PHP：只读属性
来源：http://hz.xziqi.cn/gtwaymxzbx.html

public readonly string $name
来源：http://hz.shuidangran.top/gtalctbkuf.html

[U50] PHP：构造器属性提升
来源：http://hz.zhijiandao.cn/gtczxfhycc.html

public function __construct(private int $id) {}
来源：http://hz.yuxming.cn/gtvvxfgwgu.html

[U51] PHP：数组解构
来源：http://hz.9152youxi.cn/gturpybpce.html

[$a, $b] = $arr;
来源：http://hz.guannengcc.top/gtffgdmzaj.html

[U52] PHP：箭头函数
来源：http://hz.316326.xyz/gtbtsavqur.html

$double = fn($x) => $x * 2;
来源：http://hz.nanxuanxn.top/gtiufgjwas.html

[U53] PHP：空合并运算符
来源：http://hz.yvedp.cn/gtnkqmzwkw.html

$v = $a ?? $b ?? "default";
来源：http://hz.c1oappe.top/gtblegouon.html

[U54] PHP：空安全调用
来源：http://hz.daria6918.cn/gtwhzqgwyn.html

$obj?->method()
来源：http://hz.hywenlv.cn/gtmhfgcclp.html


<!-- 参考信息 -->