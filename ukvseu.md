代发 wailian999

[S33] C++：vector 增删
来源：http://hz.dashuyun.cn/gtvmwbabew.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.snrcjt.cn/gtcpgzfexa.html

[S34] C++：遍历 vector
来源：http://hz.pengpengdd.cyou/gtqaqeaeay.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.redwolf501.top/gtfquiofmc.html

[S35] C++：map
来源：http://hz.meibo888.top/gthfxxqzxd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yongpay.top/gtdoexcxzw.html

[S36] C++：unordered_map
来源：http://hz.ywan-chungtsiang.top/gtetsmlrdz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gtsxwohrwj.html

[S37] C++：set
来源：http://hz.dianchejie.cn/gtlatkmarq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cashguo.top/gtadzhhuxn.html

[S38] C++：排序
来源：http://hz.mhx1999.top/gtvoodpuyk.html

std::sort(v.begin(), v.end());
来源：http://hz.ivvv.top/gtqfnvphbh.html

[S39] C++：自定义比较器排序
来源：http://hz.smart0.xyz/gtzrrgpchi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.snrcjt.cn/gthswnjumf.html

[S40] C++：查找元素
来源：http://hz.yangfankeji.com/gtshhplitc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.c1oappe.top/gtpcxofkja.html

[S41] C++：类与构造函数
来源：http://hz.xziqi.cn/gtsogehzyc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhijiandao.cn/gtqsksnllm.html

[S42] C++：继承与虚函数
来源：http://hz.cheryme.top/gtmorskhld.html

class B : public Base { public: void f() override {} };
来源：http://hz.ehwqpu.com/gtvjlmdsvt.html

[S43] C++：智能指针
来源：http://hz.tanke756.top/gtqwfnndfa.html

auto p = std::make_unique<int>(5);
来源：http://hz.ppjwa.cn/gtztdamfjz.html

[S44] C++：引用传参
来源：http://hz.smart0.xyz/gtlzrgpria.html

void inc(int &x) { ++x; }
来源：http://hz.gogol.net.cn/gtpntdjgtr.html

[S45] C++：lambda
来源：http://hz.xingfuxueyuan.xyz/gtfbfdzrib.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.meibo888.top/gtazocycdw.html

[S46] C++：函数模板
来源：http://hz.zhaomingkeji.xyz/gtwibvbrlb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhiwuduotai.top/gtcmzwslip.html

[S47] C++：结构化绑定遍历
来源：http://hz.xinyue.icu/gtbjqcycpv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xingfuxueyuan.xyz/gtpejkpbkr.html

[S48] C++：逐行读文件
来源：http://hz.guowangkeji.top/gtqpvliwtb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yueranfly.top/gtknsmjcpg.html

while (std::getline(in, line)) { }
来源：http://hz.tianlin.xyz/gtpppqjbnp.html

[S49] C++：写文件
来源：http://hz.haohaochexian.top/gtnwcsirhg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.haohaochexian.top/gtyggovwod.html

[S50] C++：格式化数字
来源：http://hz.zhijiandao.cn/gtusutdeeq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258888.top/gtjompseth.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangkeji.top/gtdczifxqq.html

static_cast<double>(a) / b
来源：http://hz.jinyuanbaomall.cn/gtzqgbvdom.html

[S52] C++：const 与 noexcept
来源：http://hz.ydzc1.top/gtboufcxdg.html

int size() const noexcept { return n_; }
来源：http://hz.zhijiandao.cn/gtcmzjslos.html

[S53] C++：移动语义
来源：http://hz.jlsjyb.cn/gtkmxsshml.html

std::vector<int> w = std::move(v);
来源：http://hz.zhoulong.xyz/gtoaoiqykx.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gtzwoqepjv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgufenzy.top/gtqfjvwazk.html

[S55] C++：结构化绑定
来源：http://hz.yangfankeji.com/gtmrzvtpep.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shzxlz.cn/gtvogokwsg.html

[S56] C++：optional
来源：http://hz.redwolf501.top/gtgcdmoloo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jianghu66.top/gtaumfvsxi.html

[S57] C++：编译期常量
来源：http://hz.sysykeji.top/gtokxatmsf.html

constexpr int N = 10;
来源：http://hz.yanxiufei.cn/gtimjtxbtx.html

[S58] C++：命名空间
来源：http://hz.snrcjt.cn/gthjtwzemi.html

namespace ns { int f() { return 1; } }
来源：http://hz.jyoumei.cn/gtdyopodvs.html

[S59] C++：静态断言
来源：http://hz.gzhubu.top/gtheghyqdk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhijiandao.cn/gtsagpzcdz.html

[S60] C++：遍历并删除元素
来源：http://hz.cqqwz.cn/gtrmunhsge.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yvedp.cn/gteaaettuc.html

================================================================================
来源：http://hz.yj202588.top/gtuhfpxuyl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cheryme.top/gtcnkhplzr.html

================================================================================
来源：http://hz.tian-w.cn/gtnriybbgw.html

[T01] Kotlin：Hello World
来源：http://hz.dashuyun.cn/gttpdaeybg.html

println("Hello")
来源：http://hz.c1oappe.top/gtosumeqfn.html

[T02] Kotlin：变量
来源：http://hz.shanyushiyangkeji.top/gttjirdnie.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xziqi.cn/gtgghnnizk.html

[T03] Kotlin：字符串模板
来源：http://hz.zhengqikj.top/gtkcymmvlr.html

"值: $b"
来源：http://hz.yuxming.cn/gtrmicpasu.html

[T04] Kotlin：空安全
来源：http://hz.guannengcc.top/gtctbpfsfo.html

val n: String? = null;  n?.length
来源：http://hz.jinghuilouyu.cn/gtsndqfhil.html

[T05] Kotlin：when 表达式
来源：http://hz.nanxinkj.top/gtqiyuixhp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.havefunace.top/gtptlznipc.html

[T06] Kotlin：集合映射
来源：http://hz.yanxiufei.cn/gtvchnbzwl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinghuilouyu.cn/gtrehfjkyu.html

[T07] Kotlin：集合过滤
来源：http://hz.gaohongyu789.top/gtgxuuaepo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cheryme.top/gtazpovynr.html

[T08] Kotlin：数据类
来源：http://hz.tianlin.xyz/gtsasawegg.html

data class User(val name: String, val age: Int)
来源：http://hz.gaohongyu789.top/gteailzrqu.html

[T09] Kotlin：扩展函数
来源：http://hz.smart0.xyz/gtvowdkprc.html

fun String.exclaim() = this + "!"
来源：http://hz.xinyue.icu/gtvnnlkqri.html

[T10] Kotlin：默认参数
来源：http://hz.pycfn.com/gteozyrfzc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.pycfn.com/gtxpjcshtf.html

[T11] Kotlin：协程
来源：http://hz.nanxinkj.top/gtdjeotxet.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daxiang520.top/gtutsmtyjd.html

[T12] Kotlin：解构声明
来源：http://hz.birdmap.top/gtbgottmne.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhaomingkeji.xyz/gtgbybujie.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258.top/gthnsmxjvj.html

val m = mapOf("a" to 1)
来源：http://hz.andypj.xyz/gtnxurdncr.html

[T14] Kotlin：循环
来源：http://hz.daxiang520.top/gtadwiejyk.html

for (i in 1..10) println(i)
来源：http://hz.cqqwz.cn/gtjtyxfzqf.html

[T15] Kotlin：接口
来源：http://hz.jyoumei.cn/gtkdulmthq.html

interface Shape { fun area(): Double }
来源：http://hz.yanxiufei.cn/gthqjsbncc.html

[T16] Swift：Hello World
来源：http://hz.xuetiantiany.cn/gtlvjdmmns.html

print("Hello")
来源：http://hz.zhixingplan.top/gtmhjbpblw.html

[T17] Swift：变量与常量
来源：http://hz.ybcxt.top/gtpgrafxgu.html

var a = 1;  let b = 2
来源：http://hz.cashguo.top/gtqgbgdcky.html

[T18] Swift：字符串插值
来源：http://hz.yj20258888.top/gtzbnixfap.html

"值: \(b)"
来源：http://hz.chenzaomai.com/gtztmmuztl.html

[T19] Swift：可选绑定
来源：http://hz.yuanzhike.top/gtbrcpdaoj.html

if let n = opt { print(n) }
来源：http://hz.xingfuxueyuan.xyz/gtxftwkwhx.html

[T20] Swift：数组操作
来源：http://hz.yueranfly.top/gtrlsxaaot.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gogol.net.cn/gtawzfkerj.html

[T21] Swift：遍历
来源：http://hz.zhongyouzk.top/gtiiraikxz.html

for x in a { print(x) }
来源：http://hz.yj202588.top/gtahnlnjns.html

[T22] Swift：字典
来源：http://hz.aibaodan.cn/gtyiulkpso.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xuanzx.com/gtealuuvfw.html

[T23] Swift：函数
来源：http://hz.aizwys.cn/gtksgyatul.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yuanzhike.top/gtcvbpwgcm.html

[T24] Swift：闭包
来源：http://hz.svipenyu.cn/gtshmxpjup.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.meibo888.top/gtwpzkmxpx.html

[T25] Swift：结构体
来源：http://hz.wangshuangyany.cn/gtnysluaeu.html

struct P { var x: Int }
来源：http://hz.wangshuangyany.cn/gtearcxtig.html

[T26] Swift：类与重写
来源：http://hz.xylfe.cn/gtfpeooutr.html

class A: Base { override func f() {} }
来源：http://hz.cucudq.cn/gtgwuiloeo.html

[T27] Swift：错误处理
来源：http://hz.xinyue.icu/gtfuxrjatr.html

do { try f() } catch { print(error) }
来源：http://hz.xylfe.cn/gtirggpgmg.html

[T28] Swift：枚举
来源：http://hz.hnxiangtu.top/gtppcbmwmf.html

enum Color { case red, green }
来源：http://hz.shanyushiyangtech.top/gtkkzsqvff.html

[T29] Swift：guard 提前返回
来源：http://hz.ehwqpu.com/gtkberignb.html

guard let x = opt else { return }
来源：http://hz.chenlongwang.top/gtnimfvvcb.html

[T30] Swift：协议
来源：http://hz.wangshuangyany.cn/gtxuwufuae.html

protocol Shape { func area() -> Double }
来源：http://hz.aizwys.cn/gttwvodfvz.html

[T31] Lua：Hello World
来源：http://hz.mhx1999.top/gtpjcqdmil.html

print("Hello")
来源：http://hz.yj20258.top/gtxypztahu.html

[T32] Lua：局部变量
来源：http://hz.haohaochexian.top/gtwwekubmj.html

local a = 1
来源：http://hz.sweek.top/gtdffohfbh.html

[T33] Lua：表（数组）
来源：http://hz.dashuyun.cn/gtpngmfzyv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sxryk.cn/gtzgzpytqm.html

[T34] Lua：遍历表
来源：http://hz.jinqigfzy.top/gtlogyhkbu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jqgufenzy.top/gtjqsizonr.html

[T35] Lua：字典表
来源：http://hz.ydzc1.top/gtdkwattfm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj20258.top/gtrwtnkypg.html

[T36] Lua：函数
来源：http://hz.gotoacloud.top/gtomtqyzoz.html

function add(a, b) return a + b end
来源：http://hz.yj20258888.top/gtixsscuoj.html

[T37] Lua：字符串拼接
来源：http://hz.cqqwz.cn/gtqygzqdji.html

"a" .. "b"
来源：http://hz.ehwqpu.com/gticlmknko.html

[T38] Lua：条件
来源：http://hz.vqdsnc.cn/gtodqeooqf.html

if x > 0 then print("正") end
来源：http://hz.hnqzz.top/gtpkpeznof.html

[T39] Lua：模式匹配
来源：http://hz.fengsongda.top/gtcvzzrprp.html

string.find(s, "%d+")
来源：http://hz.ivvv.top/gtnrrkkbct.html

[T40] Lua：元表
来源：http://hz.snrcjt.cn/gttdbatcxi.html

setmetatable({}, { __index = base })
来源：http://hz.zycfv.cn/gtabaqhqme.html

[T41] Perl：Hello World
来源：http://hz.xuetiantiany.cn/gtdqwoghgy.html

print "Hello\n";
来源：http://hz.ybcxt.top/gtwyonuank.html

[T42] Perl：变量类型
来源：http://hz.jinqigfzy.top/gtbxzqrhpb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shangyingyoupin.top/gtrhrfrnfq.html

[T43] Perl：字符串插值
来源：http://hz.gzhubu.top/gtesvwugfe.html

"值: $a"
来源：http://hz.zdqjudy.top/gtbleuaqmn.html

[T44] Perl：条件
来源：http://hz.ehwqpu.com/gtdwgqhvyu.html

if ($a > 0) { print "正"; }
来源：http://hz.nwbrower.top/gttmnwhjos.html

[T45] Perl：数组遍历
来源：http://hz.shanyushiyangtech.top/gtgbbdlomq.html

for my $x (@arr) { print $x; }
来源：http://hz.gotoacloud.top/gtblunagqs.html

[T46] Perl：哈希操作
来源：http://hz.jlsjyb.cn/gtprpbnfyg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhongyouzk.top/gtfwwogjxo.html

[T47] Perl：正则捕获
来源：http://hz.hysaishi.cn/gtbqcgfzbt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.meibo888.top/gtzruqnfwn.html

[T48] Perl：正则替换
来源：http://hz.jqgufenzy.top/gtomssfnxp.html

$s =~ s/old/new/g;
来源：http://hz.jyoumei.cn/gtlumlavdi.html

[T49] Perl：函数
来源：http://hz.yuxming.cn/gtwynvffvi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hnqzz.top/gtfommibxr.html

[T50] Perl：逐行读文件
来源：http://hz.bjfxy.top/gtunrthhod.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yuanzhike.top/gtoroyntva.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shuidangran.top/gtqbwqtbno.html

[T51] Scala：Hello World
来源：http://hz.jqgfzy.top/gtuevyubhk.html

println("Hello")
来源：http://hz.316326.xyz/gtkpgdsxif.html

[T52] Scala：变量
来源：http://hz.jiagoushi.top/gtcreepuyd.html

val a = 1;  var b = 2
来源：http://hz.jinqigfzy.top/gtrvypwual.html

[T53] Scala：字符串插值
来源：http://hz.cqqwz.cn/gtfpnwhuqf.html

s"值: $b"
来源：http://hz.pycfn.com/gtydabganm.html

[T54] Scala：集合映射
来源：http://hz.xuanzx.com/gtdlohuamm.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.c1oappe.top/gtmiqqohpl.html

[T55] Scala：集合过滤
来源：http://hz.jqgufenzy.top/gtsfkuytjt.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ehwqpu.com/gtfvcceudh.html

[T56] Scala：样例类
来源：http://hz.xuetiantiany.cn/gtekvxobdv.html

case class User(name: String, age: Int)
来源：http://hz.sufxvd.cn/gttarulbea.html

[T57] Scala：模式匹配
来源：http://hz.svipenyu.cn/gtlrepqaxh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.wangshuangyany.cn/gtdjmruhfk.html

[T58] Scala：函数定义
来源：http://hz.ydzc1.top/gttapdvygy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.haohaochexian.top/gtsniyoaiy.html

[T59] Scala：循环
来源：http://hz.zhaomingkeji.xyz/gthyohbbxi.html

for (i <- 1 to 10) println(i)
来源：http://hz.sweek.top/gtmmffdwdz.html

[T60] Scala：折叠
来源：http://hz.dianchejie.cn/gtbiycugay.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xingfuxueyuan.xyz/gtciuywhct.html

================================================================================
来源：http://hz.0kj1m.cn/gtapqufhul.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnqzz.top/gtfaexowhv.html

================================================================================
来源：http://hz.xziqi.cn/gtwicqxgig.html

[U01] Py：创建虚拟环境
来源：http://hz.hnxiangtu.top/gtmwazflte.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hysaishi.cn/gtqzurmllv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pycfn.com/gtrceftukm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.316326.xyz/gttuxyqamf.html

[U03] Py：加载 .env 配置
来源：http://hz.hongshengwenyu.top/gthspcqkdl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.fzhhl.top/gtlourbxpn.html

[U04] Py：变量调试打印
来源：http://hz.ydjk.org.cn/gtfjhhuvbz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.daxiang520.top/gtvvzltaej.html

[U05] Py：列表去重且保序
来源：http://hz.svipenyu.cn/gtossciklv.html

list(dict.fromkeys(arr))
来源：http://hz.nwbrower.top/gtompzziho.html

[U06] Py：合并两个字典
来源：http://hz.chenzaomai.com/gtecswqmmg.html

{**a, **b}
来源：http://hz.nanxuanxn.top/gturwbpjfv.html

[U07] Py：反转字典键值
来源：http://hz.xuetiantiany.cn/gtwsfbmwaq.html

{v: k for k, v in d.items()}
来源：http://hz.yj202588.top/gtfhhbrkbl.html

[U08] Py：展平二维列表
来源：http://hz.wangdashe.top/gtpmohyvbx.html

[y for x in nested for y in x]
来源：http://hz.jinghuilouyu.cn/gtthzfrzrq.html

[U09] Py：字典取最大值的键
来源：http://hz.havefunace.top/gtobwwqqrh.html

max(d, key=d.get)
来源：http://hz.fzhhl.top/gtpqpskqmw.html

[U10] Py：按值排序字典
来源：http://hz.ybcxt.top/gtvnksiqtb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cdnleiting.top/gteyqgkjas.html

[U11] Py：生成器表达式
来源：http://hz.yonumen.top/gtsswaelir.html

(x * 2 for x in arr)
来源：http://hz.dashuyun.cn/gtlmznwwsd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yangfankeji.com/gtvzdixkdz.html

Counter(arr).most_common(3)
来源：http://hz.havefunace.top/gtnmyfwskd.html

[U13] Py：固定长度队列
来源：http://hz.yj20258.top/gtxmdzmcyj.html

deque(maxlen=10)
来源：http://hz.shanyushiyangkeji.top/gtfzxvfxqe.html

[U14] Py：分组收集到列表
来源：http://hz.bjfxy.top/gtjbcmygbl.html

defaultdict(list)
来源：http://hz.jinghuilouyu.cn/gtmckmdbyl.html

[U15] Py：高精度计时
来源：http://hz.xylfe.cn/gtnistnbah.html

t = time.perf_counter()
来源：http://hz.tianlin.xyz/gtkkupcivy.html

[U16] Py：命令行参数解析
来源：http://hz.sufxvd.cn/gtujubooot.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.aibaodan.cn/gtlaknmiff.html

[U17] Py：初始化日志
来源：http://hz.havefunace.top/gtayparmcm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.fzhhl.top/gtngkiqugs.html

[U18] Py：预编译正则
来源：http://hz.quarkkingdee.top/gtuydwixmy.html

pat = re.compile(r"\d+")
来源：http://hz.aibaodan.cn/gtuulvvbrm.html

[U19] Py：正则替换带回调
来源：http://hz.xuetiantiany.cn/gtovijigro.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.mhx1999.top/gtwkgnuani.html

[U20] Py：缓存函数结果
来源：http://hz.aizwys.cn/gtpbeedlqy.html

@functools.lru_cache(maxsize=None)
来源：http://hz.316326.xyz/gtzvevlhad.html

[U21] Py：自定义上下文管理器
来源：http://hz.hnqzz.top/gtgirpqfxc.html

@contextlib.contextmanager
来源：http://hz.jinghuilouyu.cn/gtmovyawax.html

[U22] Py：矩阵转置
来源：http://hz.cashguo.top/gtrkxmtvxm.html

list(zip(*m))
来源：http://hz.ppjwa.cn/gtyhsicrmw.html

[U23] Py：分块读取大文件
来源：http://hz.ywan-chungtsiang.top/gtqfcmtsxl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.haohaochexian.top/gtjsvutcfu.html

[U24] Py：路径操作
来源：http://hz.havefunace.top/gtrfatznqu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yuanzhike.top/gtclrannxh.html

[U25] Py：CSV 按字典读
来源：http://hz.gotoacloud.top/gtnbfuhnce.html

csv.DictReader(f)
来源：http://hz.nanxinkj.top/gtfznkqupr.html

[U26] Py：并发下载
来源：http://hz.52xcode.cn/gtvgtbidca.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhaomingkeji.xyz/gtrgjqbwkd.html

[U27] Py：异步 HTTP
来源：http://hz.jyoumei.cn/gtussuwuww.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.0kj1m.cn/gtehtybrzg.html

[U28] Py：类型别名
来源：http://hz.jianghu66.top/gtpislqyvt.html

UserId = int
来源：http://hz.c1oappe.top/gtbvbqgztk.html

[U29] Py：属性校验
来源：http://hz.kuanghao11.cn/gtzonxsrtd.html

@property 与 @x.setter 配合
来源：http://hz.nwbrower.top/gtgmtncpmy.html

[U30] Py：数据类
来源：http://hz.chenzaomai.com/gtowjkpmxy.html

@dataclass(slots=True)
来源：http://hz.sweek.top/gtkcqzytno.html

[U31] Py：单测
来源：http://hz.chenjidiqi.icu/gtvkelyucj.html

python -m pytest -q
来源：http://hz.tanke756.top/gtpsfmjssp.html

[U32] Py：代码格式化
来源：http://hz.yj20258888.top/gtqwdybhde.html

ruff format . && ruff check --fix .
来源：http://hz.zhoulong.xyz/gtoiwfmrwf.html

[U33] Py：打包发布
来源：http://hz.smart0.xyz/gtxazcmqeo.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.wangshuangyany.cn/gtgwssvhjh.html

[U34] Py：判断编码
来源：http://hz.birdmap.top/gtyagnguch.html

chardet.detect(raw)
来源：http://hz.hongshengwenyu.top/gtgvulaxaq.html

[U35] Py：发送邮件
来源：http://hz.wangdashe.top/gtdpqicxdt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shangyingyoupin.top/gtbvesbalx.html

[U36] Py：定时任务
来源：http://hz.zhoulong.xyz/gtnjedfhqf.html

schedule.every(10).minutes.do(job)
来源：http://hz.jqgfzy.top/gtiibmvzzg.html

[U37] Py：读写 Excel
来源：http://hz.yongpay.top/gtdfvwwpmi.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.guannengcc.top/gtimjijiwl.html

[U38] Py：获取脚本所在目录
来源：http://hz.zdqjudy.top/gtywgvvslv.html

Path(__file__).resolve().parent
来源：http://hz.jqgfzy.top/gtfodacqvp.html

[U39] Py：判断是否在交互环境
来源：http://hz.mhx1999.top/gtdvatikff.html

sys.stdout.isatty()
来源：http://hz.zhiwuduotai.top/gtcbqxtklq.html

[U40] Py：打印到标准错误
来源：http://hz.sweek.top/gtbxytldyq.html

print("err", file=sys.stderr)
来源：http://hz.shanyushiyangkeji.top/gtlqlkagam.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jiagoushi.top/gtzsqyahdp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinqigfzy.top/gtvcdffrrt.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gotoacloud.top/gtklzeayom.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.birdmap.top/gtaxkkcysu.html

[U43] PHP：声明命名空间
来源：http://hz.nwbrower.top/gtvjabfork.html

namespace App\Http;
来源：http://hz.sweek.top/gttaealdnj.html

[U44] PHP：开启严格类型
来源：http://hz.redwolf501.top/gtpokbjvat.html

declare(strict_types=1);
来源：http://hz.shzxlz.cn/gtfznvgqfz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.nwbrower.top/gtrzgjgslp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtccyatmno.html

[U46] PHP：可空类型
来源：http://hz.havefunace.top/gtnsdqxutq.html

?string $name = null
来源：http://hz.zycfv.cn/gtptupuied.html

[U47] PHP：联合类型
来源：http://hz.feifeiyinyue.top/gtbooxiexd.html

int|string $id
来源：http://hz.jiagoushi.top/gtjcbhhaaj.html

[U48] PHP：纯枚举
来源：http://hz.ehwqpu.com/gtnjazrtku.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.guannengcc.top/gtqzlmfsrq.html

[U49] PHP：只读属性
来源：http://hz.chenzaomai.com/gtyjhsplsq.html

public readonly string $name
来源：http://hz.zhixingplan.top/gtgwkebjfm.html

[U50] PHP：构造器属性提升
来源：http://hz.quarkkingdee.top/gtunanycmz.html

public function __construct(private int $id) {}
来源：http://hz.gotoacloud.top/gtnrrtbeed.html

[U51] PHP：数组解构
来源：http://hz.zhengqikj.top/gtvpqgilwb.html

[$a, $b] = $arr;
来源：http://hz.redwolf501.top/gtsuxywgtv.html

[U52] PHP：箭头函数
来源：http://hz.jlsjyb.cn/gtdceidxaz.html

$double = fn($x) => $x * 2;
来源：http://hz.zhijiandao.cn/gtsjqkfrec.html

[U53] PHP：空合并运算符
来源：http://hz.ywan-chungtsiang.top/gtvwgqcder.html

$v = $a ?? $b ?? "default";
来源：http://hz.gogol.net.cn/gtjmykzulm.html

[U54] PHP：空安全调用
来源：http://hz.iojbl.cn/gtjrzyyglm.html

$obj?->method()
来源：http://hz.fzhhl.top/gtuuhhzmai.html

[U55] PHP：match 表达式
来源：http://hz.zhengqikj.top/gtetczydmu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.svipenyu.cn/gthxqzboch.html

[U56] PHP：命名参数
来源：http://hz.haohaochexian.top/gtmuxajjeo.html

f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtbizycqcl.html

[U57] PHP：字符串插值
来源：http://hz.gogol.net.cn/gtnxuctqti.html

"值: {$a}"
来源：http://hz.shuidangran.top/gtvjwnxkrh.html

[U58] PHP：数组三件套
来源：http://hz.52xcode.cn/gtnkkkforg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ydjk.org.cn/gtfiuhzrnf.html


<!-- 参考信息 -->