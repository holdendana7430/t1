代发 wailian999

#include <iostream>
来源：http://hz.yj20258.top/gtpktuyreo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hongshengwenyu.top/gtstwyiwpq.html

[S32] C++：字符串
来源：http://hz.ydjk.org.cn/gtnnaorkuc.html

std::string s = "hi";  s += "!";
来源：http://hz.52xcode.cn/gtpquzaeay.html

[S33] C++：vector 增删
来源：http://hz.zhaomingkeji.xyz/gtqujtnzor.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gogol.net.cn/gtxljupvfb.html

[S34] C++：遍历 vector
来源：http://hz.ivvv.top/gtlxmygvft.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shanyushiyangtech.top/gtauxpuxmm.html

[S35] C++：map
来源：http://hz.birdmap.top/gtxgqygpjc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hammf.cn/gtioqqyvio.html

[S36] C++：unordered_map
来源：http://hz.ybcxt.top/gttrnpcxdx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtbznxhvhx.html

[S37] C++：set
来源：http://hz.snrcjt.cn/gtqrxxyczh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.pengpengdd.cyou/gtlsiazieo.html

[S38] C++：排序
来源：http://hz.shanyushiyangtech.top/gtyufrovui.html

std::sort(v.begin(), v.end());
来源：http://hz.sxryk.cn/gtodubitdt.html

[S39] C++：自定义比较器排序
来源：http://hz.jinqigufen.top/gtpzddryhi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shangyingyoupin.top/gtqpfxdmvz.html

[S40] C++：查找元素
来源：http://hz.jinghuilouyu.cn/gtoxdykjdz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tianlin.xyz/gthhmzrvkx.html

[S41] C++：类与构造函数
来源：http://hz.zhaomingkeji.xyz/gtampzqlwl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.0kj1m.cn/gthqlioakf.html

[S42] C++：继承与虚函数
来源：http://hz.ppjwa.cn/gtjiidnnkd.html

class B : public Base { public: void f() override {} };
来源：http://hz.birdmap.top/gtrbntilod.html

[S43] C++：智能指针
来源：http://hz.zhaomingkeji.xyz/gtfoqgoxhl.html

auto p = std::make_unique<int>(5);
来源：http://hz.aizwys.cn/gtpbaxedkd.html

[S44] C++：引用传参
来源：http://hz.shuidangran.top/gtdomgkyvi.html

void inc(int &x) { ++x; }
来源：http://hz.fengsongda.top/gtqlgkjxgs.html

[S45] C++：lambda
来源：http://hz.nwbrower.top/gtjytxgahd.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ywan-chungtsiang.top/gtduzuriwf.html

[S46] C++：函数模板
来源：http://hz.smart0.xyz/gtgdcyvfqo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhiwuduotai.top/gtqkbplppn.html

[S47] C++：结构化绑定遍历
来源：http://hz.andypj.xyz/gtwgcxhblz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nanxuanxn.top/gtabwzyrdk.html

[S48] C++：逐行读文件
来源：http://hz.meibo888.top/gtbjxhbguh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cqqwz.cn/gtykrofsuo.html

while (std::getline(in, line)) { }
来源：http://hz.zhengqikj.top/gtwfqaqmmw.html

[S49] C++：写文件
来源：http://hz.yueranfly.top/gtaiekvjtn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnqzz.top/gtbnbcpylx.html

[S50] C++：格式化数字
来源：http://hz.shanyushiyangkeji.top/gtenaoojcv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.c1oappe.top/gttyniinvt.html

[S51] C++：显式类型转换
来源：http://hz.cucudq.cn/gthftxcvzk.html

static_cast<double>(a) / b
来源：http://hz.haohaochexian.top/gthulrgcvm.html

[S52] C++：const 与 noexcept
来源：http://hz.0kj1m.cn/gtylxiwtnf.html

int size() const noexcept { return n_; }
来源：http://hz.meibo888.top/gtiimszuxp.html

[S53] C++：移动语义
来源：http://hz.hywenlv.cn/gtagkeorxt.html

std::vector<int> w = std::move(v);
来源：http://hz.cucudq.cn/gtjrolhenp.html

[S54] C++：异常处理
来源：http://hz.zhiwuduotai.top/gtugmuprkn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj202588.top/gtxldkmqye.html

[S55] C++：结构化绑定
来源：http://hz.chenlongwang.top/gtfwdamajt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuanzhike.top/gtpgwechev.html

[S56] C++：optional
来源：http://hz.zhaomingkeji.xyz/gtrbktzbzu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhiwuduotai.top/gtsyfgmhyb.html

[S57] C++：编译期常量
来源：http://hz.mhx1999.top/gtoaobuvum.html

constexpr int N = 10;
来源：http://hz.zhengqikj.top/gtbpiuqzqv.html

[S58] C++：命名空间
来源：http://hz.316326.xyz/gtvdnibwju.html

namespace ns { int f() { return 1; } }
来源：http://hz.hongshengwenyu.top/gtzblynxne.html

[S59] C++：静态断言
来源：http://hz.fzhhl.top/gtppamrixn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yangfankeji.com/gtgrtinmrw.html

[S60] C++：遍历并删除元素
来源：http://hz.cdnleiting.top/gtbfjsmkcl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nwbrower.top/gtejbsuzbw.html

================================================================================
来源：http://hz.hywenlv.cn/gtwjdvgmag.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sweek.top/gtvgvwrhcf.html

================================================================================
来源：http://hz.kuanghao11.cn/gtavnmdyeq.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangkeji.top/gtfwuljbqx.html

println("Hello")
来源：http://hz.zhiwuduotai.top/gtvdllbhkm.html

[T02] Kotlin：变量
来源：http://hz.hywenlv.cn/gtmxwucxvq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxuanxn.top/gtwumkcfde.html

[T03] Kotlin：字符串模板
来源：http://hz.wangdashe.top/gttoifnapm.html

"值: $b"
来源：http://hz.smart0.xyz/gtmkkkxvwq.html

[T04] Kotlin：空安全
来源：http://hz.yongpay.top/gtnucgukbc.html

val n: String? = null;  n?.length
来源：http://hz.ybcxt.top/gtcrjcxull.html

[T05] Kotlin：when 表达式
来源：http://hz.kuanghao11.cn/gtimcrzsil.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tanke756.top/gtnnwjfwyb.html

[T06] Kotlin：集合映射
来源：http://hz.cdnleiting.top/gtwnhhexdh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinqigfzy.top/gtralyntqp.html

[T07] Kotlin：集合过滤
来源：http://hz.ehwqpu.com/gtbijunauc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigfzy.top/gtzhdtdxep.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangtech.top/gtultyxjbo.html

data class User(val name: String, val age: Int)
来源：http://hz.ppjwa.cn/gtrcjwlywd.html

[T09] Kotlin：扩展函数
来源：http://hz.cdnleiting.top/gttxuovyad.html

fun String.exclaim() = this + "!"
来源：http://hz.kuanghao11.cn/gtymqfykcm.html

[T10] Kotlin：默认参数
来源：http://hz.guannengcc.top/gtkkmidlpy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yonumen.top/gtxosmoltf.html

[T11] Kotlin：协程
来源：http://hz.guannengcc.top/gtjrmqxunn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.pycfn.com/gtunzxvozn.html

[T12] Kotlin：解构声明
来源：http://hz.sysykeji.top/gtmhgtvfmd.html

val (a, b) = Pair(1, 2)
来源：http://hz.tanke756.top/gtzbzqmuwz.html

[T13] Kotlin：只读 Map
来源：http://hz.quarkkingdee.top/gtkbiquown.html

val m = mapOf("a" to 1)
来源：http://hz.316326.xyz/gtomfwgubx.html

[T14] Kotlin：循环
来源：http://hz.xuanzx.com/gtznjqtfar.html

for (i in 1..10) println(i)
来源：http://hz.cqqwz.cn/gtqzuttdjb.html

[T15] Kotlin：接口
来源：http://hz.316326.xyz/gtonquypre.html

interface Shape { fun area(): Double }
来源：http://hz.yangfankeji.com/gtlaaxkyyh.html

[T16] Swift：Hello World
来源：http://hz.9152youxi.cn/gtynnsdahg.html

print("Hello")
来源：http://hz.xuetiantiany.cn/gtumvwlccv.html

[T17] Swift：变量与常量
来源：http://hz.ydzc1.top/gtggxwupmw.html

var a = 1;  let b = 2
来源：http://hz.xinyue.icu/gtkrsauvjd.html

[T18] Swift：字符串插值
来源：http://hz.iojbl.cn/gttniystax.html

"值: \(b)"
来源：http://hz.guowangkeji.top/gtpoyxbjkg.html

[T19] Swift：可选绑定
来源：http://hz.yj202588.top/gtioqpclqv.html

if let n = opt { print(n) }
来源：http://hz.jyoumei.cn/gtpsmnuogj.html

[T20] Swift：数组操作
来源：http://hz.guannengcc.top/gtyjrembsc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.iojbl.cn/gttlgbpxvy.html

[T21] Swift：遍历
来源：http://hz.snrcjt.cn/gthpwcywye.html

for x in a { print(x) }
来源：http://hz.pengpengdd.cyou/gtkdtvfojn.html

[T22] Swift：字典
来源：http://hz.fzhhl.top/gtpekihoxk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shuidangran.top/gtlftbyjqi.html

[T23] Swift：函数
来源：http://hz.jianghu66.top/gtgctssfms.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shanyushiyangtech.top/gttkquhcpp.html

[T24] Swift：闭包
来源：http://hz.zhijiandao.cn/gtifqvhsxs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ywan-chungtsiang.top/gtxxzfrwib.html

[T25] Swift：结构体
来源：http://hz.yonumen.top/gtbqjplnku.html

struct P { var x: Int }
来源：http://hz.yueranfly.top/gtbxoullra.html

[T26] Swift：类与重写
来源：http://hz.shanyushiyangkeji.top/gtenmicmlr.html

class A: Base { override func f() {} }
来源：http://hz.tian-w.cn/gtjdfopddt.html

[T27] Swift：错误处理
来源：http://hz.mhx1999.top/gtfcoaiofk.html

do { try f() } catch { print(error) }
来源：http://hz.aizwys.cn/gtafhlzosu.html

[T28] Swift：枚举
来源：http://hz.snrcjt.cn/gtwvgelric.html

enum Color { case red, green }
来源：http://hz.kuanghao11.cn/gtstbhfanx.html

[T29] Swift：guard 提前返回
来源：http://hz.tian-w.cn/gtktbrombr.html

guard let x = opt else { return }
来源：http://hz.pengpengdd.cyou/gtblcsfrvv.html

[T30] Swift：协议
来源：http://hz.andypj.xyz/gtxkpomsaf.html

protocol Shape { func area() -> Double }
来源：http://hz.nanxuanxn.top/gtwwbfjqyg.html

[T31] Lua：Hello World
来源：http://hz.ydjk.org.cn/gtrkswkcbk.html

print("Hello")
来源：http://hz.jyoumei.cn/gtkekktnvq.html

[T32] Lua：局部变量
来源：http://hz.ywan-chungtsiang.top/gtqksiovkd.html

local a = 1
来源：http://hz.zhongyouzk.top/gtrfczftcm.html

[T33] Lua：表（数组）
来源：http://hz.jiagoushi.top/gtnbvmnqmb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.tianlin.xyz/gtnhmtnkne.html

[T34] Lua：遍历表
来源：http://hz.yj20258.top/gtclamhppg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinqigufen.top/gttriqqnzy.html

[T35] Lua：字典表
来源：http://hz.svipenyu.cn/gtodponngj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yueranfly.top/gtrojndxbk.html

[T36] Lua：函数
来源：http://hz.wangdashe.top/gtndazjeys.html

function add(a, b) return a + b end
来源：http://hz.hysaishi.cn/gtlpzlxgcm.html

[T37] Lua：字符串拼接
来源：http://hz.svipenyu.cn/gtoprkvhmj.html

"a" .. "b"
来源：http://hz.0kj1m.cn/gthguamzis.html

[T38] Lua：条件
来源：http://hz.ydzc1.top/gthafiyndr.html

if x > 0 then print("正") end
来源：http://hz.yuanzhike.top/gtobotpxeh.html

[T39] Lua：模式匹配
来源：http://hz.yj20258888.top/gtgchtbqrl.html

string.find(s, "%d+")
来源：http://hz.zhijiandao.cn/gtqoucetni.html

[T40] Lua：元表
来源：http://hz.bjfxy.top/gtkzfyijps.html

setmetatable({}, { __index = base })
来源：http://hz.ybcxt.top/gtjjeauwaa.html

[T41] Perl：Hello World
来源：http://hz.yonumen.top/gthhvmycxs.html

print "Hello\n";
来源：http://hz.andypj.xyz/gtfquvykbj.html

[T42] Perl：变量类型
来源：http://hz.nanxuanxn.top/gtpqfmarcu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj20258888.top/gtzqrmlnss.html

[T43] Perl：字符串插值
来源：http://hz.cashguo.top/gtbuibjkqd.html

"值: $a"
来源：http://hz.xinyue.icu/gtazdgtkvg.html

[T44] Perl：条件
来源：http://hz.xylfe.cn/gtvvcawlzs.html

if ($a > 0) { print "正"; }
来源：http://hz.yanxiufei.cn/gtrvcymlaq.html

[T45] Perl：数组遍历
来源：http://hz.gaohongyu789.top/gtuveprmfa.html

for my $x (@arr) { print $x; }
来源：http://hz.ybcxt.top/gtynqxqpkh.html

[T46] Perl：哈希操作
来源：http://hz.ivvv.top/gthjqtqedn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ehwqpu.com/gtkyvonwfu.html

[T47] Perl：正则捕获
来源：http://hz.aizwys.cn/gtcepuaylq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.snrcjt.cn/gtvljooajz.html

[T48] Perl：正则替换
来源：http://hz.zhijiandao.cn/gtaylwsbkw.html

$s =~ s/old/new/g;
来源：http://hz.birdmap.top/gtfbwuztit.html

[T49] Perl：函数
来源：http://hz.cashguo.top/gtjvvgofsw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinqigfzy.top/gtacvsphdt.html

[T50] Perl：逐行读文件
来源：http://hz.yj20258.top/gtdhbegzhu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.birdmap.top/gtirmeditj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.9152youxi.cn/gtoqeiznjq.html

[T51] Scala：Hello World
来源：http://hz.daria6918.cn/gtvrzvybut.html

println("Hello")
来源：http://hz.yj20258.top/gtvfftnxij.html

[T52] Scala：变量
来源：http://hz.ydzc1.top/gtjicvjqxd.html

val a = 1;  var b = 2
来源：http://hz.cucudq.cn/gtvdpbbsxa.html

[T53] Scala：字符串插值
来源：http://hz.hnqzz.top/gtmmtjcvyj.html

s"值: $b"
来源：http://hz.shanyushiyangkeji.top/gtrdngqfms.html

[T54] Scala：集合映射
来源：http://hz.wangdashe.top/gtbvmfwqxb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shuidangran.top/gtfaudhjep.html

[T55] Scala：集合过滤
来源：http://hz.nwbrower.top/gtmeghqvhk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.wangdashe.top/gtzpspezbb.html

[T56] Scala：样例类
来源：http://hz.jlsjyb.cn/gtqzfcwnhf.html

case class User(name: String, age: Int)
来源：http://hz.ppjwa.cn/gtdyknhwwg.html

[T57] Scala：模式匹配
来源：http://hz.feifeiyinyue.top/gtidblnvbx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ydjk.org.cn/gtlvhupsxb.html

[T58] Scala：函数定义
来源：http://hz.shanyushiyangtech.top/gtpnjeemfg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yongpay.top/gtfvzqscyc.html

[T59] Scala：循环
来源：http://hz.jinqigfzy.top/gtkhksmufl.html

for (i <- 1 to 10) println(i)
来源：http://hz.52xcode.cn/gtvlxbjznp.html

[T60] Scala：折叠
来源：http://hz.gaohongyu789.top/gtksobqqzf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.kuanghao11.cn/gtedabntmk.html

================================================================================
来源：http://hz.gotoacloud.top/gtgnbweiid.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.mhx1999.top/gtyhjlbuvu.html

================================================================================
来源：http://hz.daria6918.cn/gtkkrypmqu.html

[U01] Py：创建虚拟环境
来源：http://hz.ywan-chungtsiang.top/gtebqzwozg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cqqwz.cn/gtqpmhxudt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.meibo888.top/gtnmfhcpee.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yj202588.top/gtfmwzoaed.html

[U03] Py：加载 .env 配置
来源：http://hz.snrcjt.cn/gtlpsrjqhm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.0kj1m.cn/gtmqeimanr.html

[U04] Py：变量调试打印
来源：http://hz.bjfxy.top/gtmwxykrji.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hnqzz.top/gtqtmpdmxm.html

[U05] Py：列表去重且保序
来源：http://hz.tianlin.xyz/gtxoluixwj.html

list(dict.fromkeys(arr))
来源：http://hz.jqgufenzy.top/gtrkulkxgb.html

[U06] Py：合并两个字典
来源：http://hz.xuetiantiany.cn/gtgwvscfdd.html

{**a, **b}
来源：http://hz.hammf.cn/gtxpbhiblv.html

[U07] Py：反转字典键值
来源：http://hz.316326.xyz/gtjwkqhqdc.html

{v: k for k, v in d.items()}
来源：http://hz.316326.xyz/gtdjxtftmb.html

[U08] Py：展平二维列表
来源：http://hz.gaohongyu789.top/gtvzvumfay.html

[y for x in nested for y in x]
来源：http://hz.dashuyun.cn/gtnamamknu.html

[U09] Py：字典取最大值的键
来源：http://hz.jianghu66.top/gtpapsmfnq.html

max(d, key=d.get)
来源：http://hz.yvedp.cn/gtkushlcue.html

[U10] Py：按值排序字典
来源：http://hz.cashguo.top/gtyxxhcigg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.kuanghao11.cn/gtndkcozzn.html

[U11] Py：生成器表达式
来源：http://hz.nanxinkj.top/gtughcdmzi.html

(x * 2 for x in arr)
来源：http://hz.nanxuanxn.top/gtsivqacvr.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.9152youxi.cn/gtmkffnbem.html

Counter(arr).most_common(3)
来源：http://hz.jqgfzy.top/gtpvxrwzvi.html

[U13] Py：固定长度队列
来源：http://hz.hammf.cn/gtzafyybsw.html

deque(maxlen=10)
来源：http://hz.haohaochexian.top/gtncqjbjrr.html

[U14] Py：分组收集到列表
来源：http://hz.zhoulong.xyz/gtfevkydmf.html

defaultdict(list)
来源：http://hz.xinyue.icu/gtwnvpvhev.html

[U15] Py：高精度计时
来源：http://hz.zdqjudy.top/gtbgmwptns.html

t = time.perf_counter()
来源：http://hz.smart0.xyz/gthmbginvx.html

[U16] Py：命令行参数解析
来源：http://hz.jyoumei.cn/gtkgxxhyny.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.aizwys.cn/gtlxuwgtuw.html

[U17] Py：初始化日志
来源：http://hz.zhiwuduotai.top/gtlwmguidr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.meibo888.top/gtaujuhjjy.html

[U18] Py：预编译正则
来源：http://hz.zhijiandao.cn/gtulfkatdq.html

pat = re.compile(r"\d+")
来源：http://hz.pengpengdd.cyou/gtnhkmxdzc.html

[U19] Py：正则替换带回调
来源：http://hz.zhiwuduotai.top/gtgwbtybdl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zdqjudy.top/gtolozuflo.html

[U20] Py：缓存函数结果
来源：http://hz.zdqjudy.top/gtsevvjfqs.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj20258.top/gtcjwxzalk.html

[U21] Py：自定义上下文管理器
来源：http://hz.tian-w.cn/gtwamedzqh.html

@contextlib.contextmanager
来源：http://hz.yvedp.cn/gtasikhkcs.html

[U22] Py：矩阵转置
来源：http://hz.xuetiantiany.cn/gtttxgpcbc.html

list(zip(*m))
来源：http://hz.cashguo.top/gtqebkgwmm.html

[U23] Py：分块读取大文件
来源：http://hz.zhongyouzk.top/gttrtuagwc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hysaishi.cn/gtiljzkpnn.html

[U24] Py：路径操作
来源：http://hz.zhoulong.xyz/gtbsieptxc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.iojbl.cn/gtpbvgbfrw.html

[U25] Py：CSV 按字典读
来源：http://hz.daria6918.cn/gtsbudryti.html

csv.DictReader(f)
来源：http://hz.guowangkeji.top/gtokqciplo.html

[U26] Py：并发下载
来源：http://hz.svipenyu.cn/gtvkirtbtg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xingfuxueyuan.xyz/gtswijkzjz.html

[U27] Py：异步 HTTP
来源：http://hz.ydzc1.top/gtazfvtqxd.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ehwqpu.com/gtutzrrwqh.html

[U28] Py：类型别名
来源：http://hz.wangdashe.top/gtyhpkglis.html

UserId = int
来源：http://hz.jlsjyb.cn/gtnsphjhtm.html

[U29] Py：属性校验
来源：http://hz.zhongyouzk.top/gtjbiyrcpw.html

@property 与 @x.setter 配合
来源：http://hz.birdmap.top/gtqpjyortg.html

[U30] Py：数据类
来源：http://hz.bjfxy.top/gtwrhvdqkq.html

@dataclass(slots=True)
来源：http://hz.smart0.xyz/gtnmydbugb.html

[U31] Py：单测
来源：http://hz.haohaochexian.top/gtrookktcl.html

python -m pytest -q
来源：http://hz.zhixingplan.top/gtklhhkacj.html

[U32] Py：代码格式化
来源：http://hz.chenlongwang.top/gtnvsdmdzx.html

ruff format . && ruff check --fix .
来源：http://hz.gogol.net.cn/gtumswibzk.html

[U33] Py：打包发布
来源：http://hz.dianchejie.cn/gtwqfbhieg.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jianghu66.top/gtnjsbfvzs.html

[U34] Py：判断编码
来源：http://hz.ydzc1.top/gtcreehodv.html

chardet.detect(raw)
来源：http://hz.aibaodan.cn/gtlezinfyl.html

[U35] Py：发送邮件
来源：http://hz.kuanghao11.cn/gtiiawwgzl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xingfuxueyuan.xyz/gtwruypybv.html

[U36] Py：定时任务
来源：http://hz.jinyuanbaomall.cn/gtfteljhuf.html

schedule.every(10).minutes.do(job)
来源：http://hz.316326.xyz/gtmusxrsrj.html

[U37] Py：读写 Excel
来源：http://hz.zhoulong.xyz/gtoimaenxi.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ydzc1.top/gtelfndvvy.html

[U38] Py：获取脚本所在目录
来源：http://hz.hfpthk.cn/gthdeldqjc.html

Path(__file__).resolve().parent
来源：http://hz.nwbrower.top/gtrmrckaaj.html

[U39] Py：判断是否在交互环境
来源：http://hz.sxryk.cn/gtihaxgmmi.html

sys.stdout.isatty()
来源：http://hz.ybcxt.top/gtfijctumw.html

[U40] Py：打印到标准错误
来源：http://hz.daria6918.cn/gtpkylabdg.html

print("err", file=sys.stderr)
来源：http://hz.svipenyu.cn/gtsxmqrefa.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenzaomai.com/gtumcwwiyo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.haohaochexian.top/gtzaopvgag.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.feifeiyinyue.top/gtkfpbjbhc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.0kj1m.cn/gtlwdhwzyo.html

[U43] PHP：声明命名空间
来源：http://hz.jqgfzy.top/gtxqlgoodh.html

namespace App\Http;
来源：http://hz.jinyuanbaomall.cn/gtolqyihcb.html

[U44] PHP：开启严格类型
来源：http://hz.hammf.cn/gtjnqqzuvd.html

declare(strict_types=1);
来源：http://hz.pycfn.com/gtyfroerdc.html

[U45] PHP：类型声明与返回类型
来源：http://hz.gogol.net.cn/gtleaqspmc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtxiivwhkf.html

[U46] PHP：可空类型
来源：http://hz.hfpthk.cn/gtucweqtjq.html

?string $name = null
来源：http://hz.0kj1m.cn/gtzxfedlzj.html

[U47] PHP：联合类型
来源：http://hz.quarkkingdee.top/gtokafqqrs.html

int|string $id
来源：http://hz.zhaomingkeji.xyz/gtkyeunlmx.html

[U48] PHP：纯枚举
来源：http://hz.nanxuanxn.top/gtyywfgjuk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gogol.net.cn/gtcfnxgcqw.html

[U49] PHP：只读属性
来源：http://hz.cheryme.top/gtvfufjwfk.html

public readonly string $name
来源：http://hz.jqgufenzy.top/gtnvxhdvyb.html

[U50] PHP：构造器属性提升
来源：http://hz.cdnleiting.top/gtyxdibnfa.html

public function __construct(private int $id) {}
来源：http://hz.yonumen.top/gtoyocsqfi.html

[U51] PHP：数组解构
来源：http://hz.zhongyouzk.top/gteeyqqegq.html

[$a, $b] = $arr;
来源：http://hz.zycfv.cn/gtwxqwlmko.html

[U52] PHP：箭头函数
来源：http://hz.tian-w.cn/gtwevkfsjc.html

$double = fn($x) => $x * 2;
来源：http://hz.tanke756.top/gtovufbylf.html

[U53] PHP：空合并运算符
来源：http://hz.pycfn.com/gtbnecubvl.html

$v = $a ?? $b ?? "default";
来源：http://hz.ehwqpu.com/gtoaeejpxi.html

[U54] PHP：空安全调用
来源：http://hz.hammf.cn/gtqbozgvex.html

$obj?->method()
来源：http://hz.yonumen.top/gtgdfhwedm.html

[U55] PHP：match 表达式
来源：http://hz.chenjidiqi.icu/gtqdcdgosn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xuetiantiany.cn/gtdyekfbpy.html

[U56] PHP：命名参数
来源：http://hz.cdnleiting.top/gtrfajlxsk.html

f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtlaqjnvql.html


<!-- 参考信息 -->