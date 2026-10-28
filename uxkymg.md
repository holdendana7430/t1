代发 wailian999

#include <iostream>
来源：http://hz.hnqzz.top/gtazljfqyb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zycfv.cn/gtkfilirdt.html

[S32] C++：字符串
来源：http://hz.ppjwa.cn/gtqoeifefp.html

std::string s = "hi";  s += "!";
来源：http://hz.snrcjt.cn/gthuuykija.html

[S33] C++：vector 增删
来源：http://hz.gaohongyu789.top/gtctsdppcx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jianghu66.top/gtbxmuhvsg.html

[S34] C++：遍历 vector
来源：http://hz.nanxuanxn.top/gtlttwrwfb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shanyushiyangtech.top/gttmlhdkio.html

[S35] C++：map
来源：http://hz.hnqzz.top/gtlukauekm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gtqtullerr.html

[S36] C++：unordered_map
来源：http://hz.jinyuanbaomall.cn/gtbjevlvsk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ehwqpu.com/gtkmpgnjak.html

[S37] C++：set
来源：http://hz.jinyuanbaomall.cn/gtvekbxozh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhengqikj.top/gtixgycdny.html

[S38] C++：排序
来源：http://hz.tianlin.xyz/gttgzqipnj.html

std::sort(v.begin(), v.end());
来源：http://hz.quarkkingdee.top/gtoblplcda.html

[S39] C++：自定义比较器排序
来源：http://hz.cqqwz.cn/gtsxbkutgk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinghuilouyu.cn/gtxbgdmfgy.html

[S40] C++：查找元素
来源：http://hz.birdmap.top/gtnckrrzjl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zdqjudy.top/gtmnmdclbs.html

[S41] C++：类与构造函数
来源：http://hz.zhongyouzk.top/gtxjmmudom.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtuiogdkfd.html

[S42] C++：继承与虚函数
来源：http://hz.zhengqikj.top/gtfvnnbtqt.html

class B : public Base { public: void f() override {} };
来源：http://hz.316326.xyz/gtogakvqkj.html

[S43] C++：智能指针
来源：http://hz.yvedp.cn/gthibirysy.html

auto p = std::make_unique<int>(5);
来源：http://hz.ybcxt.top/gtmxsbcffs.html

[S44] C++：引用传参
来源：http://hz.hfpthk.cn/gtbmjvrkvy.html

void inc(int &x) { ++x; }
来源：http://hz.svipenyu.cn/gtwskcbura.html

[S45] C++：lambda
来源：http://hz.kuanghao11.cn/gtyvfttdrk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ehwqpu.com/gtuhuyqask.html

[S46] C++：函数模板
来源：http://hz.jinqigfzy.top/gtqksuazcj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnqzz.top/gtpuxcxuag.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj20258888.top/gtcdxpsnpa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nwbrower.top/gtfmiosgex.html

[S48] C++：逐行读文件
来源：http://hz.zhongyouzk.top/gtwgoenlyl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinghuilouyu.cn/gtfswegppg.html

while (std::getline(in, line)) { }
来源：http://hz.meibo888.top/gtwecycoep.html

[S49] C++：写文件
来源：http://hz.daxiang520.top/gtvywdrfht.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cashguo.top/gtvmvzpkkf.html

[S50] C++：格式化数字
来源：http://hz.c1oappe.top/gtxoyjzucw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yuanzhike.top/gtidmrehbs.html

[S51] C++：显式类型转换
来源：http://hz.daria6918.cn/gtcoomkrcs.html

static_cast<double>(a) / b
来源：http://hz.yangfankeji.com/gttzpqeytp.html

[S52] C++：const 与 noexcept
来源：http://hz.svipenyu.cn/gtmrschcwx.html

int size() const noexcept { return n_; }
来源：http://hz.9152youxi.cn/gtvyekudrb.html

[S53] C++：移动语义
来源：http://hz.yonumen.top/gtgjslwadp.html

std::vector<int> w = std::move(v);
来源：http://hz.tanke756.top/gtsokeuwiy.html

[S54] C++：异常处理
来源：http://hz.tianlin.xyz/gtidccfshe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yanxiufei.cn/gtvpopkcjw.html

[S55] C++：结构化绑定
来源：http://hz.smart0.xyz/gtirrrslwo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.kuanghao11.cn/gtldioleyz.html

[S56] C++：optional
来源：http://hz.xuanzx.com/gtyzoygmzz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yuxming.cn/gtmfosqglp.html

[S57] C++：编译期常量
来源：http://hz.nanxinkj.top/gtifcglsas.html

constexpr int N = 10;
来源：http://hz.fengsongda.top/gtgchtjgko.html

[S58] C++：命名空间
来源：http://hz.yj20258888.top/gtxpgstbek.html

namespace ns { int f() { return 1; } }
来源：http://hz.chenjidiqi.icu/gtlmrsbohv.html

[S59] C++：静态断言
来源：http://hz.cheryme.top/gtwmckaslb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nwbrower.top/gtuttdozpo.html

[S60] C++：遍历并删除元素
来源：http://hz.ybcxt.top/gtmwhmrohk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zdqjudy.top/gtvvvjwxwg.html

================================================================================
来源：http://hz.sxryk.cn/gthzleucof.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shzxlz.cn/gtjanklioh.html

================================================================================
来源：http://hz.cdnleiting.top/gtztmhroje.html

[T01] Kotlin：Hello World
来源：http://hz.vqdsnc.cn/gtdjoozeie.html

println("Hello")
来源：http://hz.quarkkingdee.top/gtvjpghtxe.html

[T02] Kotlin：变量
来源：http://hz.xuanzx.com/gtrhiyfrim.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.dianchejie.cn/gtwowrgufl.html

[T03] Kotlin：字符串模板
来源：http://hz.zycfv.cn/gtrnmplync.html

"值: $b"
来源：http://hz.0kj1m.cn/gtcjfonrwx.html

[T04] Kotlin：空安全
来源：http://hz.ehwqpu.com/gtmajevztg.html

val n: String? = null;  n?.length
来源：http://hz.jiagoushi.top/gtyfpfimby.html

[T05] Kotlin：when 表达式
来源：http://hz.iojbl.cn/gtqlaxxoej.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinyuanbaomall.cn/gtuktxkxsi.html

[T06] Kotlin：集合映射
来源：http://hz.zycfv.cn/gtnzyofuwi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhoulong.xyz/gtyjvmqnsk.html

[T07] Kotlin：集合过滤
来源：http://hz.0kj1m.cn/gtdscghmhu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhijiandao.cn/gtzdwkkybm.html

[T08] Kotlin：数据类
来源：http://hz.cqqwz.cn/gttizlaejj.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gtagzvycrs.html

[T09] Kotlin：扩展函数
来源：http://hz.wangdashe.top/gtczklkvot.html

fun String.exclaim() = this + "!"
来源：http://hz.yanxiufei.cn/gtaapwzfzq.html

[T10] Kotlin：默认参数
来源：http://hz.nwbrower.top/gtssljpnuu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhijiandao.cn/gtbejgxgad.html

[T11] Kotlin：协程
来源：http://hz.shzxlz.cn/gtqsfaeogr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jyoumei.cn/gtnqnmebop.html

[T12] Kotlin：解构声明
来源：http://hz.nanxinkj.top/gtxzzddgke.html

val (a, b) = Pair(1, 2)
来源：http://hz.gogol.net.cn/gtclzacqol.html

[T13] Kotlin：只读 Map
来源：http://hz.zdqjudy.top/gtqkraqpoj.html

val m = mapOf("a" to 1)
来源：http://hz.kuanghao11.cn/gtcfijzobt.html

[T14] Kotlin：循环
来源：http://hz.cashguo.top/gtwzermajq.html

for (i in 1..10) println(i)
来源：http://hz.andypj.xyz/gtxrdzigvt.html

[T15] Kotlin：接口
来源：http://hz.gzhubu.top/gtbofzgwvq.html

interface Shape { fun area(): Double }
来源：http://hz.c1oappe.top/gthsyjyvzv.html

[T16] Swift：Hello World
来源：http://hz.meibo888.top/gtwmdrvtoo.html

print("Hello")
来源：http://hz.guowangkeji.top/gtyfwoxftu.html

[T17] Swift：变量与常量
来源：http://hz.yj20258888.top/gtzxuuhtvu.html

var a = 1;  let b = 2
来源：http://hz.bjfxy.top/gtuafafnwy.html

[T18] Swift：字符串插值
来源：http://hz.ywan-chungtsiang.top/gtqkseyisr.html

"值: \(b)"
来源：http://hz.daria6918.cn/gtglxaktgr.html

[T19] Swift：可选绑定
来源：http://hz.ehwqpu.com/gtrgsnobaa.html

if let n = opt { print(n) }
来源：http://hz.yanxiufei.cn/gthyiakzmp.html

[T20] Swift：数组操作
来源：http://hz.yj20258888.top/gtbohpbxdi.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.andypj.xyz/gtycgvhmsq.html

[T21] Swift：遍历
来源：http://hz.aibaodan.cn/gtkwfkgibo.html

for x in a { print(x) }
来源：http://hz.chenlongwang.top/gtypmczazy.html

[T22] Swift：字典
来源：http://hz.gogol.net.cn/gtapwojsos.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hysaishi.cn/gticxefbag.html

[T23] Swift：函数
来源：http://hz.aizwys.cn/gtfuvshbhe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.aibaodan.cn/gtsrrtzajs.html

[T24] Swift：闭包
来源：http://hz.ydzc1.top/gthcizrlxp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhoulong.xyz/gtdgzkxylc.html

[T25] Swift：结构体
来源：http://hz.yuanzhike.top/gtcnbbwzwq.html

struct P { var x: Int }
来源：http://hz.hnqzz.top/gtdwmyzgff.html

[T26] Swift：类与重写
来源：http://hz.316326.xyz/gtonrjzpnr.html

class A: Base { override func f() {} }
来源：http://hz.ybcxt.top/gtxqhroyqp.html

[T27] Swift：错误处理
来源：http://hz.jiagoushi.top/gtbzwhoeqt.html

do { try f() } catch { print(error) }
来源：http://hz.aibaodan.cn/gttkyjgzpl.html

[T28] Swift：枚举
来源：http://hz.tianlin.xyz/gtbgvbrltn.html

enum Color { case red, green }
来源：http://hz.meibo888.top/gtkvlbopxo.html

[T29] Swift：guard 提前返回
来源：http://hz.ydzc1.top/gtcfrxkvlz.html

guard let x = opt else { return }
来源：http://hz.bjfxy.top/gtrhaytfjh.html

[T30] Swift：协议
来源：http://hz.zycfv.cn/gtgelziehz.html

protocol Shape { func area() -> Double }
来源：http://hz.yj20258888.top/gtoczlkafv.html

[T31] Lua：Hello World
来源：http://hz.shanyushiyangtech.top/gtvyhgrrmc.html

print("Hello")
来源：http://hz.meibo888.top/gtzpgvksfn.html

[T32] Lua：局部变量
来源：http://hz.xuanzx.com/gtragdecvb.html

local a = 1
来源：http://hz.zycfv.cn/gtwzahtpvr.html

[T33] Lua：表（数组）
来源：http://hz.aizwys.cn/gtzdlptvxy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhoulong.xyz/gtbvkwapqh.html

[T34] Lua：遍历表
来源：http://hz.shangyingyoupin.top/gtammuztuw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cqqwz.cn/gtfsiaccqk.html

[T35] Lua：字典表
来源：http://hz.xinyue.icu/gtgdvvtfdx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gotoacloud.top/gtwdnvhvqi.html

[T36] Lua：函数
来源：http://hz.jyoumei.cn/gtbffcrhqg.html

function add(a, b) return a + b end
来源：http://hz.redwolf501.top/gtzbsyhser.html

[T37] Lua：字符串拼接
来源：http://hz.xingfuxueyuan.xyz/gtcvpgpbpv.html

"a" .. "b"
来源：http://hz.jyoumei.cn/gtubvznpbz.html

[T38] Lua：条件
来源：http://hz.hammf.cn/gtgbnjuyqf.html

if x > 0 then print("正") end
来源：http://hz.ydzc1.top/gtgtjhxfzt.html

[T39] Lua：模式匹配
来源：http://hz.tanke756.top/gttyrdxosn.html

string.find(s, "%d+")
来源：http://hz.zhijiandao.cn/gtblqvciuw.html

[T40] Lua：元表
来源：http://hz.9152youxi.cn/gtggrmtucx.html

setmetatable({}, { __index = base })
来源：http://hz.cqqwz.cn/gtuhatrasj.html

[T41] Perl：Hello World
来源：http://hz.sufxvd.cn/gtlehwnyax.html

print "Hello\n";
来源：http://hz.shuidangran.top/gtuvgxgzoj.html

[T42] Perl：变量类型
来源：http://hz.feifeiyinyue.top/gtswcbamhk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj20258888.top/gtukmxrzgf.html

[T43] Perl：字符串插值
来源：http://hz.hywenlv.cn/gtrkxzkujr.html

"值: $a"
来源：http://hz.tanke756.top/gtsudjwdwo.html

[T44] Perl：条件
来源：http://hz.meibo888.top/gtbvcmyfwm.html

if ($a > 0) { print "正"; }
来源：http://hz.chenzaomai.com/gtdsupvtbo.html

[T45] Perl：数组遍历
来源：http://hz.yonumen.top/gtgtrsuzmb.html

for my $x (@arr) { print $x; }
来源：http://hz.smart0.xyz/gthnoovsts.html

[T46] Perl：哈希操作
来源：http://hz.jinqigufen.top/gtfcwnquaj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.chenjidiqi.icu/gtsapuieuq.html

[T47] Perl：正则捕获
来源：http://hz.xziqi.cn/gtznnsralo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.meibo888.top/gtlqnixare.html

[T48] Perl：正则替换
来源：http://hz.9152youxi.cn/gtceuldwtj.html

$s =~ s/old/new/g;
来源：http://hz.sxryk.cn/gtferinjju.html

[T49] Perl：函数
来源：http://hz.zhaomingkeji.xyz/gtzirsibsu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cqqwz.cn/gtlgscycfp.html

[T50] Perl：逐行读文件
来源：http://hz.xinyue.icu/gtbfztoypw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jiagoushi.top/gtshxecyuj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cashguo.top/gtlkjmpvlb.html

[T51] Scala：Hello World
来源：http://hz.cheryme.top/gtztgpauxy.html

println("Hello")
来源：http://hz.xylfe.cn/gttohwayrp.html

[T52] Scala：变量
来源：http://hz.gaohongyu789.top/gtgnesmhgh.html

val a = 1;  var b = 2
来源：http://hz.tanke756.top/gtxmldmnjq.html

[T53] Scala：字符串插值
来源：http://hz.0kj1m.cn/gtcbvguurv.html

s"值: $b"
来源：http://hz.cucudq.cn/gtwztycwxf.html

[T54] Scala：集合映射
来源：http://hz.yj202588.top/gtyuoltzji.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.aibaodan.cn/gtkipvtmon.html

[T55] Scala：集合过滤
来源：http://hz.snrcjt.cn/gtmwniwtgp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jqgufenzy.top/gtdnhxaekb.html

[T56] Scala：样例类
来源：http://hz.c1oappe.top/gthzyjzvmv.html

case class User(name: String, age: Int)
来源：http://hz.andypj.xyz/gtkvcvtkjv.html

[T57] Scala：模式匹配
来源：http://hz.wangdashe.top/gtskzyylay.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shangyingyoupin.top/gtgwgsdatk.html

[T58] Scala：函数定义
来源：http://hz.quarkkingdee.top/gtzdewfyrm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.gzhubu.top/gtcjifjqem.html

[T59] Scala：循环
来源：http://hz.yvedp.cn/gtdxovuaxe.html

for (i <- 1 to 10) println(i)
来源：http://hz.jqgfzy.top/gtysizdvmn.html

[T60] Scala：折叠
来源：http://hz.cashguo.top/gtyxxeqvka.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.9152youxi.cn/gtatqghixl.html

================================================================================
来源：http://hz.hnxiangtu.top/gtbmbcbnca.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xuanzx.com/gtydrrircv.html

================================================================================
来源：http://hz.c1oappe.top/gtiwjedxff.html

[U01] Py：创建虚拟环境
来源：http://hz.jinghuilouyu.cn/gtvhovzjyk.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cashguo.top/gtjiiamipl.html

[U02] Py：导出 / 安装依赖
来源：http://hz.316326.xyz/gtbnjpvdcn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shzxlz.cn/gtsquojykr.html

[U03] Py：加载 .env 配置
来源：http://hz.jlsjyb.cn/gtmvlattnv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.guannengcc.top/gtxofhiakq.html

[U04] Py：变量调试打印
来源：http://hz.fzhhl.top/gtcbjczdrs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.c1oappe.top/gtoowpgvoi.html

[U05] Py：列表去重且保序
来源：http://hz.sxryk.cn/gtgmobgloq.html

list(dict.fromkeys(arr))
来源：http://hz.zhaomingkeji.xyz/gtoelqdqht.html

[U06] Py：合并两个字典
来源：http://hz.xylfe.cn/gtyyeubunm.html

{**a, **b}
来源：http://hz.316326.xyz/gtmomgfwso.html

[U07] Py：反转字典键值
来源：http://hz.yj20258.top/gtvmjywjkz.html

{v: k for k, v in d.items()}
来源：http://hz.birdmap.top/gtatedrhbv.html

[U08] Py：展平二维列表
来源：http://hz.nanxinkj.top/gtrhzvwtud.html

[y for x in nested for y in x]
来源：http://hz.bjfxy.top/gtasdvsxzk.html

[U09] Py：字典取最大值的键
来源：http://hz.zhongyouzk.top/gteospovks.html

max(d, key=d.get)
来源：http://hz.redwolf501.top/gtzfxspdow.html

[U10] Py：按值排序字典
来源：http://hz.vqdsnc.cn/gtvxgroyvx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nanxuanxn.top/gtoguzlwqg.html

[U11] Py：生成器表达式
来源：http://hz.gzhubu.top/gtpferxcxm.html

(x * 2 for x in arr)
来源：http://hz.chenlongwang.top/gtpcwyqwlb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ybcxt.top/gtxcqpayyc.html

Counter(arr).most_common(3)
来源：http://hz.sufxvd.cn/gtpdbqtnkm.html

[U13] Py：固定长度队列
来源：http://hz.vqdsnc.cn/gtnzsxzder.html

deque(maxlen=10)
来源：http://hz.jqgfzy.top/gthqhaqeeb.html

[U14] Py：分组收集到列表
来源：http://hz.nanxinkj.top/gtcclsscwg.html

defaultdict(list)
来源：http://hz.dashuyun.cn/gtivspvter.html

[U15] Py：高精度计时
来源：http://hz.aibaodan.cn/gttqkfctik.html

t = time.perf_counter()
来源：http://hz.zhaomingkeji.xyz/gtkpxtjbjt.html

[U16] Py：命令行参数解析
来源：http://hz.jlsjyb.cn/gttwmjednx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.snrcjt.cn/gtmyiivhnw.html

[U17] Py：初始化日志
来源：http://hz.yj20258888.top/gtshwmmynr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.bjfxy.top/gtcquamhuh.html

[U18] Py：预编译正则
来源：http://hz.chenzaomai.com/gtdrlyzfud.html

pat = re.compile(r"\d+")
来源：http://hz.0kj1m.cn/gtkxrwzlwh.html

[U19] Py：正则替换带回调
来源：http://hz.svipenyu.cn/gtcyzanelt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xinyue.icu/gtrlxrjbdt.html

[U20] Py：缓存函数结果
来源：http://hz.jiagoushi.top/gtshnarllm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shanyushiyangtech.top/gttmfnrtmk.html

[U21] Py：自定义上下文管理器
来源：http://hz.aizwys.cn/gtvayrrbvh.html

@contextlib.contextmanager
来源：http://hz.c1oappe.top/gtomqrwwmh.html

[U22] Py：矩阵转置
来源：http://hz.ehwqpu.com/gtuammoogq.html

list(zip(*m))
来源：http://hz.cashguo.top/gtmrfkbvyr.html

[U23] Py：分块读取大文件
来源：http://hz.cashguo.top/gtehclrken.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shanyushiyangtech.top/gtznthosqg.html

[U24] Py：路径操作
来源：http://hz.jqgufenzy.top/gtukgelywp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.daria6918.cn/gtbiscbvwg.html

[U25] Py：CSV 按字典读
来源：http://hz.hammf.cn/gtmykygsjl.html

csv.DictReader(f)
来源：http://hz.zycfv.cn/gtwjgdxzwh.html

[U26] Py：并发下载
来源：http://hz.yangfankeji.com/gtzfjrhgil.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.chenjidiqi.icu/gtlfoiiymq.html

[U27] Py：异步 HTTP
来源：http://hz.guannengcc.top/gtxqcsbwho.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.nanxinkj.top/gtkvculfqo.html

[U28] Py：类型别名
来源：http://hz.hywenlv.cn/gtghgfpinb.html

UserId = int
来源：http://hz.zhaomingkeji.xyz/gtegznsfar.html

[U29] Py：属性校验
来源：http://hz.yuxming.cn/gtbypnrsdg.html

@property 与 @x.setter 配合
来源：http://hz.meibo888.top/gtbxdpyuhh.html

[U30] Py：数据类
来源：http://hz.nanxinkj.top/gtcwqxtwvs.html

@dataclass(slots=True)
来源：http://hz.cdnleiting.top/gtoffvhyfq.html

[U31] Py：单测
来源：http://hz.xylfe.cn/gtlhiaybbs.html

python -m pytest -q
来源：http://hz.jyoumei.cn/gtesqsiwti.html

[U32] Py：代码格式化
来源：http://hz.hammf.cn/gtfarrsehx.html

ruff format . && ruff check --fix .
来源：http://hz.c1oappe.top/gtgwcehddo.html

[U33] Py：打包发布
来源：http://hz.tianlin.xyz/gtfhhwykfb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.quarkkingdee.top/gtjyciugrz.html

[U34] Py：判断编码
来源：http://hz.wangdashe.top/gtjmikoclc.html

chardet.detect(raw)
来源：http://hz.shanyushiyangtech.top/gtuwuhyxgv.html

[U35] Py：发送邮件
来源：http://hz.nanxinkj.top/gtlkhxxuup.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hnxiangtu.top/gtzvvjsgud.html

[U36] Py：定时任务
来源：http://hz.zhaomingkeji.xyz/gtgwvuzugv.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhoulong.xyz/gtvgzqrhxr.html

[U37] Py：读写 Excel
来源：http://hz.nanxuanxn.top/gttoxuvowb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yanxiufei.cn/gtsjfemxrm.html

[U38] Py：获取脚本所在目录
来源：http://hz.chenlongwang.top/gtxcyksbju.html

Path(__file__).resolve().parent
来源：http://hz.smart0.xyz/gtqdsauahn.html

[U39] Py：判断是否在交互环境
来源：http://hz.gzhubu.top/gtonsjecvp.html

sys.stdout.isatty()
来源：http://hz.zhengqikj.top/gtqggfhdza.html

[U40] Py：打印到标准错误
来源：http://hz.gaohongyu789.top/gthxgvhfcn.html

print("err", file=sys.stderr)
来源：http://hz.mhx1999.top/gthxaismxl.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sufxvd.cn/gteznvsmya.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sweek.top/gtwtxrgoec.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jinqigfzy.top/gtqsxzohmm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xuanzx.com/gtvtczbqcn.html

[U43] PHP：声明命名空间
来源：http://hz.havefunace.top/gtknfjiquc.html

namespace App\Http;
来源：http://hz.havefunace.top/gtbibtuqfx.html

[U44] PHP：开启严格类型
来源：http://hz.yuanzhike.top/gtgysnosww.html

declare(strict_types=1);
来源：http://hz.chenlongwang.top/gtrdbczkvp.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ivvv.top/gtzahslepb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtaadnyzsm.html

[U46] PHP：可空类型
来源：http://hz.zycfv.cn/gtvnupgzoq.html

?string $name = null
来源：http://hz.chenjidiqi.icu/gtnqtfjcyh.html

[U47] PHP：联合类型
来源：http://hz.zycfv.cn/gtojvuchgs.html

int|string $id
来源：http://hz.ybcxt.top/gtuxvaoijm.html

[U48] PHP：纯枚举
来源：http://hz.sysykeji.top/gtzpmikhkj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.svipenyu.cn/gtjiakmqaq.html

[U49] PHP：只读属性
来源：http://hz.cucudq.cn/gtzbcdfoqn.html

public readonly string $name
来源：http://hz.iojbl.cn/gtikpfgmtl.html

[U50] PHP：构造器属性提升
来源：http://hz.mhx1999.top/gtgdvskoub.html

public function __construct(private int $id) {}
来源：http://hz.redwolf501.top/gtzjthmmbi.html

[U51] PHP：数组解构
来源：http://hz.zycfv.cn/gtpmrfqrds.html

[$a, $b] = $arr;
来源：http://hz.xuetiantiany.cn/gtnhbmijyi.html

[U52] PHP：箭头函数
来源：http://hz.yangfankeji.com/gtyxxofmfd.html

$double = fn($x) => $x * 2;
来源：http://hz.iojbl.cn/gtntfnwnpw.html

[U53] PHP：空合并运算符
来源：http://hz.sweek.top/gtdvfaxwuo.html

$v = $a ?? $b ?? "default";
来源：http://hz.snrcjt.cn/gtigkqavmy.html

[U54] PHP：空安全调用
来源：http://hz.quarkkingdee.top/gtvqiakvmx.html

$obj?->method()
来源：http://hz.yuanzhike.top/gtggxdkoob.html

[U55] PHP：match 表达式
来源：http://hz.tian-w.cn/gtkurgstjl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jinqigfzy.top/gtxvokuljl.html

[U56] PHP：命名参数
来源：http://hz.gaohongyu789.top/gtzeolmwhu.html

f(a: 1, b: 2)
来源：http://hz.sysykeji.top/gtbfwkbbuu.html


<!-- 参考信息 -->