代发 wailian999

[S35] C++：map
来源：http://hz.haohaochexian.top/gtmcetmrur.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuanzx.com/gtxpnonolq.html

[S36] C++：unordered_map
来源：http://hz.zhongyouzk.top/gttnpsbukq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zdqjudy.top/gthvtunxvv.html

[S37] C++：set
来源：http://hz.guannengcc.top/gtubsxhwaa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.52xcode.cn/gtzzxqimce.html

[S38] C++：排序
来源：http://hz.snrcjt.cn/gtsxvhmjwo.html

std::sort(v.begin(), v.end());
来源：http://hz.gzhubu.top/gtmtccbnok.html

[S39] C++：自定义比较器排序
来源：http://hz.zhixingplan.top/gtztktlfui.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cashguo.top/gtiloniytw.html

[S40] C++：查找元素
来源：http://hz.52xcode.cn/gtgvnszyvw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ybcxt.top/gtihbkqvsh.html

[S41] C++：类与构造函数
来源：http://hz.fengsongda.top/gtlkwjrzqr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shanyushiyangtech.top/gtbtigsefo.html

[S42] C++：继承与虚函数
来源：http://hz.yongpay.top/gtwlzlogsr.html

class B : public Base { public: void f() override {} };
来源：http://hz.cucudq.cn/gtvkhrujyv.html

[S43] C++：智能指针
来源：http://hz.jyoumei.cn/gtfadejjil.html

auto p = std::make_unique<int>(5);
来源：http://hz.pycfn.com/gtujynuwox.html

[S44] C++：引用传参
来源：http://hz.ehwqpu.com/gtkxjuqcdf.html

void inc(int &x) { ++x; }
来源：http://hz.hnqzz.top/gttdgmjxsu.html

[S45] C++：lambda
来源：http://hz.zhengqikj.top/gttdhqtlci.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sxryk.cn/gtrvkewdyy.html

[S46] C++：函数模板
来源：http://hz.zhixingplan.top/gtlrfzpzns.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jlsjyb.cn/gtaqeajgul.html

[S47] C++：结构化绑定遍历
来源：http://hz.ivvv.top/gtgalblnxn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yongpay.top/gtacjjmoqf.html

[S48] C++：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtkrmbdjhl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgfzy.top/gtsnxiipzq.html

while (std::getline(in, line)) { }
来源：http://hz.zhixingplan.top/gttqpakthr.html

[S49] C++：写文件
来源：http://hz.sufxvd.cn/gtsfjclypo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daxiang520.top/gtbkowjryt.html

[S50] C++：格式化数字
来源：http://hz.ehwqpu.com/gtddgrjbmi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.bjfxy.top/gtnaahrahk.html

[S51] C++：显式类型转换
来源：http://hz.shzxlz.cn/gtznvzwbhl.html

static_cast<double>(a) / b
来源：http://hz.c1oappe.top/gtlvoddyfd.html

[S52] C++：const 与 noexcept
来源：http://hz.haohaochexian.top/gtvnzkqbic.html

int size() const noexcept { return n_; }
来源：http://hz.ydzc1.top/gtiurmrtzm.html

[S53] C++：移动语义
来源：http://hz.zhijiandao.cn/gtnbyvvvpm.html

std::vector<int> w = std::move(v);
来源：http://hz.dashuyun.cn/gtthxpooxz.html

[S54] C++：异常处理
来源：http://hz.ehwqpu.com/gtphwifwhu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.havefunace.top/gtxtxbwfxv.html

[S55] C++：结构化绑定
来源：http://hz.yj20258888.top/gtyepvkfsd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cheryme.top/gtwtkrozbq.html

[S56] C++：optional
来源：http://hz.mhx1999.top/gtaejfmyvs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aizwys.cn/gtwbvvvbhu.html

[S57] C++：编译期常量
来源：http://hz.kuanghao11.cn/gtynofdbvr.html

constexpr int N = 10;
来源：http://hz.wangdashe.top/gthnvjmvom.html

[S58] C++：命名空间
来源：http://hz.xziqi.cn/gtkezwpidr.html

namespace ns { int f() { return 1; } }
来源：http://hz.quarkkingdee.top/gtzmdxzzaz.html

[S59] C++：静态断言
来源：http://hz.nanxuanxn.top/gtsemgutum.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.wangshuangyany.cn/gtnbjwfpfj.html

[S60] C++：遍历并删除元素
来源：http://hz.zhiwuduotai.top/gttodutvno.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.wangdashe.top/gtxfuenbvp.html

================================================================================
来源：http://hz.bjfxy.top/gtrelhierl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj202588.top/gtopceykjx.html

================================================================================
来源：http://hz.cdnleiting.top/gtcwswjnhb.html

[T01] Kotlin：Hello World
来源：http://hz.zhixingplan.top/gtmoukmeyr.html

println("Hello")
来源：http://hz.andypj.xyz/gtqwrnuxfu.html

[T02] Kotlin：变量
来源：http://hz.gaohongyu789.top/gtkbujivfy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gaohongyu789.top/gtsgacciia.html

[T03] Kotlin：字符串模板
来源：http://hz.jqgufenzy.top/gtvugbrwfq.html

"值: $b"
来源：http://hz.yueranfly.top/gtbulgygfq.html

[T04] Kotlin：空安全
来源：http://hz.xuetiantiany.cn/gtfbaarhbd.html

val n: String? = null;  n?.length
来源：http://hz.c1oappe.top/gtpqeuxzct.html

[T05] Kotlin：when 表达式
来源：http://hz.yj20258.top/gtetgcfvqu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhongyouzk.top/gtogjkbwdn.html

[T06] Kotlin：集合映射
来源：http://hz.tian-w.cn/gtqevuiwzb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.pycfn.com/gtbtxlsabo.html

[T07] Kotlin：集合过滤
来源：http://hz.cdnleiting.top/gtcckkkrci.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.kuanghao11.cn/gtnoaoxelb.html

[T08] Kotlin：数据类
来源：http://hz.mhx1999.top/gtrpiyzzlj.html

data class User(val name: String, val age: Int)
来源：http://hz.hongshengwenyu.top/gtyfzvhvcg.html

[T09] Kotlin：扩展函数
来源：http://hz.gzhubu.top/gtviczgqzx.html

fun String.exclaim() = this + "!"
来源：http://hz.cashguo.top/gtrfehvlco.html

[T10] Kotlin：默认参数
来源：http://hz.pycfn.com/gtprlhexqx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.52xcode.cn/gtaqpgvfrf.html

[T11] Kotlin：协程
来源：http://hz.aibaodan.cn/gtkftgnlge.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.dashuyun.cn/gtjjmeonnt.html

[T12] Kotlin：解构声明
来源：http://hz.wangshuangyany.cn/gtouakptyk.html

val (a, b) = Pair(1, 2)
来源：http://hz.kuanghao11.cn/gtexffsphm.html

[T13] Kotlin：只读 Map
来源：http://hz.feifeiyinyue.top/gtmnxjfxor.html

val m = mapOf("a" to 1)
来源：http://hz.tanke756.top/gtmuahwevg.html

[T14] Kotlin：循环
来源：http://hz.cheryme.top/gtisymjcpx.html

for (i in 1..10) println(i)
来源：http://hz.zycfv.cn/gtjusdyvli.html

[T15] Kotlin：接口
来源：http://hz.ydzc1.top/gtypfmbbap.html

interface Shape { fun area(): Double }
来源：http://hz.shangyingyoupin.top/gtnjwrktdi.html

[T16] Swift：Hello World
来源：http://hz.hnxiangtu.top/gtxvlhalle.html

print("Hello")
来源：http://hz.dianchejie.cn/gtvttryidy.html

[T17] Swift：变量与常量
来源：http://hz.cheryme.top/gttzyambsg.html

var a = 1;  let b = 2
来源：http://hz.zhongyouzk.top/gtayhsrpws.html

[T18] Swift：字符串插值
来源：http://hz.ehwqpu.com/gttkgpbssm.html

"值: \(b)"
来源：http://hz.svipenyu.cn/gtvglawbxs.html

[T19] Swift：可选绑定
来源：http://hz.jqgfzy.top/gtsicjrgjp.html

if let n = opt { print(n) }
来源：http://hz.sysykeji.top/gtzmemnjcj.html

[T20] Swift：数组操作
来源：http://hz.yueranfly.top/gtfpogbxqp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yuxming.cn/gtauxvsacl.html

[T21] Swift：遍历
来源：http://hz.yvedp.cn/gtdgiafefi.html

for x in a { print(x) }
来源：http://hz.chenzaomai.com/gtnwbvxrbt.html

[T22] Swift：字典
来源：http://hz.yueranfly.top/gtlvgshdlv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxinkj.top/gtzvsogfqi.html

[T23] Swift：函数
来源：http://hz.yongpay.top/gtnhnqmipm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yueranfly.top/gtedepxijq.html

[T24] Swift：闭包
来源：http://hz.jinyuanbaomall.cn/gtojhzrifw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.guannengcc.top/gtgaiuvwel.html

[T25] Swift：结构体
来源：http://hz.ivvv.top/gthlymmwrz.html

struct P { var x: Int }
来源：http://hz.fzhhl.top/gtncprhrtg.html

[T26] Swift：类与重写
来源：http://hz.jqgufenzy.top/gtuuehadlk.html

class A: Base { override func f() {} }
来源：http://hz.fzhhl.top/gtedtwqiis.html

[T27] Swift：错误处理
来源：http://hz.yj202588.top/gtwoxgcuom.html

do { try f() } catch { print(error) }
来源：http://hz.xziqi.cn/gtzgeupnau.html

[T28] Swift：枚举
来源：http://hz.snrcjt.cn/gtzcjlkabx.html

enum Color { case red, green }
来源：http://hz.aizwys.cn/gtrsnmlajd.html

[T29] Swift：guard 提前返回
来源：http://hz.yj202588.top/gtztgnoigx.html

guard let x = opt else { return }
来源：http://hz.316326.xyz/gtgoooofwx.html

[T30] Swift：协议
来源：http://hz.hywenlv.cn/gtmbzyvxea.html

protocol Shape { func area() -> Double }
来源：http://hz.guowangkeji.top/gtnrfsigve.html

[T31] Lua：Hello World
来源：http://hz.yuxming.cn/gtdhfjbytv.html

print("Hello")
来源：http://hz.nwbrower.top/gtdjimmlag.html

[T32] Lua：局部变量
来源：http://hz.jqgufenzy.top/gtaywexnyc.html

local a = 1
来源：http://hz.yj20258.top/gtjkfhancn.html

[T33] Lua：表（数组）
来源：http://hz.yj202588.top/gtpryaysmp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhixingplan.top/gtqafwfrjb.html

[T34] Lua：遍历表
来源：http://hz.gogol.net.cn/gtnhkjxcqu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.havefunace.top/gtsdkssbbx.html

[T35] Lua：字典表
来源：http://hz.c1oappe.top/gtdsjdzbsx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jyoumei.cn/gtiwlaqzfx.html

[T36] Lua：函数
来源：http://hz.nanxuanxn.top/gtbjyuchff.html

function add(a, b) return a + b end
来源：http://hz.xuetiantiany.cn/gtgjxsqlsb.html

[T37] Lua：字符串拼接
来源：http://hz.vqdsnc.cn/gtslsdsevd.html

"a" .. "b"
来源：http://hz.xuetiantiany.cn/gtcsdtvzti.html

[T38] Lua：条件
来源：http://hz.jyoumei.cn/gtacvqfeom.html

if x > 0 then print("正") end
来源：http://hz.pycfn.com/gtcnpozrfr.html

[T39] Lua：模式匹配
来源：http://hz.yuanzhike.top/gtqdlmrcpx.html

string.find(s, "%d+")
来源：http://hz.vqdsnc.cn/gtqzstoxid.html

[T40] Lua：元表
来源：http://hz.zhijiandao.cn/gtxezfavgy.html

setmetatable({}, { __index = base })
来源：http://hz.hnqzz.top/gtdpebhipp.html

[T41] Perl：Hello World
来源：http://hz.sxryk.cn/gtuphudyxd.html

print "Hello\n";
来源：http://hz.kuanghao11.cn/gtszwxfrcy.html

[T42] Perl：变量类型
来源：http://hz.xinyue.icu/gtheeucodh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yonumen.top/gtbcrmourc.html

[T43] Perl：字符串插值
来源：http://hz.mhx1999.top/gthdfzoeor.html

"值: $a"
来源：http://hz.jiagoushi.top/gtkixdyobb.html

[T44] Perl：条件
来源：http://hz.yanxiufei.cn/gttsmxwebd.html

if ($a > 0) { print "正"; }
来源：http://hz.kuanghao11.cn/gtmhjtuelv.html

[T45] Perl：数组遍历
来源：http://hz.yangfankeji.com/gtpysjbabd.html

for my $x (@arr) { print $x; }
来源：http://hz.zhongyouzk.top/gtgyzvpvjc.html

[T46] Perl：哈希操作
来源：http://hz.gogol.net.cn/gtsymsaxqi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.guannengcc.top/gtjgvviazf.html

[T47] Perl：正则捕获
来源：http://hz.xziqi.cn/gtfliunmgy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ehwqpu.com/gtvwzzljvf.html

[T48] Perl：正则替换
来源：http://hz.ybcxt.top/gtmgmrspfc.html

$s =~ s/old/new/g;
来源：http://hz.meibo888.top/gtdaqzjmbt.html

[T49] Perl：函数
来源：http://hz.yuanzhike.top/gtkkkhggai.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtylpmdtox.html

[T50] Perl：逐行读文件
来源：http://hz.cheryme.top/gtkxdpsovj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sweek.top/gtsroglwbp.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xuanzx.com/gtyhvwfrwy.html

[T51] Scala：Hello World
来源：http://hz.jinghuilouyu.cn/gtpjtzlhpx.html

println("Hello")
来源：http://hz.cashguo.top/gtqczqmixl.html

[T52] Scala：变量
来源：http://hz.xuetiantiany.cn/gtpxkfvmrp.html

val a = 1;  var b = 2
来源：http://hz.cdnleiting.top/gtyomadndv.html

[T53] Scala：字符串插值
来源：http://hz.ywan-chungtsiang.top/gtcavrlrfk.html

s"值: $b"
来源：http://hz.havefunace.top/gteqvbldio.html

[T54] Scala：集合映射
来源：http://hz.zhijiandao.cn/gtaoenusza.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cashguo.top/gteyuaglia.html

[T55] Scala：集合过滤
来源：http://hz.pengpengdd.cyou/gtzokvzkrq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yj20258.top/gteommhpzq.html

[T56] Scala：样例类
来源：http://hz.wangdashe.top/gtujeuhzqp.html

case class User(name: String, age: Int)
来源：http://hz.sufxvd.cn/gtcjzsuwsn.html

[T57] Scala：模式匹配
来源：http://hz.aibaodan.cn/gtxshikvjl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhengqikj.top/gtpzfspajx.html

[T58] Scala：函数定义
来源：http://hz.zdqjudy.top/gtvlokqfjc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cdnleiting.top/gtejblefir.html

[T59] Scala：循环
来源：http://hz.ppjwa.cn/gtqsoynlau.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhongyouzk.top/gtlqutxvqa.html

[T60] Scala：折叠
来源：http://hz.jlsjyb.cn/gtarvrdnyp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ybcxt.top/gtmttugusi.html

================================================================================
来源：http://hz.ydjk.org.cn/gtphojgolg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnxiangtu.top/gtjykzoyqp.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtjyysxaaw.html

[U01] Py：创建虚拟环境
来源：http://hz.hywenlv.cn/gtzosilkfe.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hysaishi.cn/gtreuphhba.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shuidangran.top/gtnvrxfvta.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yongpay.top/gtfwmkplif.html

[U03] Py：加载 .env 配置
来源：http://hz.dianchejie.cn/gtjhjadkle.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ydzc1.top/gtmbwezurs.html

[U04] Py：变量调试打印
来源：http://hz.zycfv.cn/gthmkaxeak.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zdqjudy.top/gtagnfkcdy.html

[U05] Py：列表去重且保序
来源：http://hz.smart0.xyz/gtckjljlxv.html

list(dict.fromkeys(arr))
来源：http://hz.nwbrower.top/gtlhowbnvd.html

[U06] Py：合并两个字典
来源：http://hz.gaohongyu789.top/gtnvaanyxt.html

{**a, **b}
来源：http://hz.wangshuangyany.cn/gtuujvxqwg.html

[U07] Py：反转字典键值
来源：http://hz.ybcxt.top/gttloeqmil.html

{v: k for k, v in d.items()}
来源：http://hz.sufxvd.cn/gtwtiedjen.html

[U08] Py：展平二维列表
来源：http://hz.zhaomingkeji.xyz/gtxpstlunt.html

[y for x in nested for y in x]
来源：http://hz.pycfn.com/gtkkdivjyh.html

[U09] Py：字典取最大值的键
来源：http://hz.zhoulong.xyz/gtgmwykknl.html

max(d, key=d.get)
来源：http://hz.jqgufenzy.top/gtnxpecacx.html

[U10] Py：按值排序字典
来源：http://hz.ivvv.top/gthkkyktxv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cdnleiting.top/gtemjwvvdv.html

[U11] Py：生成器表达式
来源：http://hz.xingfuxueyuan.xyz/gtqopypgss.html

(x * 2 for x in arr)
来源：http://hz.316326.xyz/gtangaavuu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.svipenyu.cn/gthwdhsesm.html

Counter(arr).most_common(3)
来源：http://hz.jyoumei.cn/gtlvahwfzg.html

[U13] Py：固定长度队列
来源：http://hz.nanxinkj.top/gtqadxwrox.html

deque(maxlen=10)
来源：http://hz.yanxiufei.cn/gtchzzerhr.html

[U14] Py：分组收集到列表
来源：http://hz.zhijiandao.cn/gtxxycmwur.html

defaultdict(list)
来源：http://hz.nwbrower.top/gtaanyszwz.html

[U15] Py：高精度计时
来源：http://hz.hammf.cn/gtubwlywcu.html

t = time.perf_counter()
来源：http://hz.guannengcc.top/gtafuychfl.html

[U16] Py：命令行参数解析
来源：http://hz.jianghu66.top/gtdgeiczgg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sxryk.cn/gtaleoqqdh.html

[U17] Py：初始化日志
来源：http://hz.shuidangran.top/gtclcdfobl.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shanyushiyangtech.top/gtrcconprw.html

[U18] Py：预编译正则
来源：http://hz.nwbrower.top/gthyausbrz.html

pat = re.compile(r"\d+")
来源：http://hz.hfpthk.cn/gtsydzpbrv.html

[U19] Py：正则替换带回调
来源：http://hz.hfpthk.cn/gtfredirpr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cdnleiting.top/gtpnjblxix.html

[U20] Py：缓存函数结果
来源：http://hz.jianghu66.top/gtetsqzpmx.html

@functools.lru_cache(maxsize=None)
来源：http://hz.tian-w.cn/gtqzpdlnzk.html

[U21] Py：自定义上下文管理器
来源：http://hz.smart0.xyz/gtagzmofrk.html

@contextlib.contextmanager
来源：http://hz.chenzaomai.com/gtclfdeciq.html

[U22] Py：矩阵转置
来源：http://hz.zhengqikj.top/gtawndrmuz.html

list(zip(*m))
来源：http://hz.yanxiufei.cn/gtcxkwwiyz.html

[U23] Py：分块读取大文件
来源：http://hz.hysaishi.cn/gthxyuxfvj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yongpay.top/gtzqtmzyob.html

[U24] Py：路径操作
来源：http://hz.jinghuilouyu.cn/gtikzvrxxo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenlongwang.top/gtxfolhhuo.html

[U25] Py：CSV 按字典读
来源：http://hz.feifeiyinyue.top/gtcdgslpko.html

csv.DictReader(f)
来源：http://hz.bjfxy.top/gtvoljcgho.html

[U26] Py：并发下载
来源：http://hz.guowangkeji.top/gtjviqmbxb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.aibaodan.cn/gtfhaeueya.html

[U27] Py：异步 HTTP
来源：http://hz.yuanzhike.top/gtjzukskbd.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sweek.top/gtmshgtmdm.html

[U28] Py：类型别名
来源：http://hz.chenjidiqi.icu/gtfdopexhd.html

UserId = int
来源：http://hz.yueranfly.top/gtbptunbyc.html

[U29] Py：属性校验
来源：http://hz.chenzaomai.com/gtjqwymhul.html

@property 与 @x.setter 配合
来源：http://hz.aibaodan.cn/gtjsrevmqz.html

[U30] Py：数据类
来源：http://hz.haohaochexian.top/gtbuxqandy.html

@dataclass(slots=True)
来源：http://hz.hywenlv.cn/gttvrnrlfi.html

[U31] Py：单测
来源：http://hz.sysykeji.top/gtccupchdr.html

python -m pytest -q
来源：http://hz.ivvv.top/gticyezahm.html

[U32] Py：代码格式化
来源：http://hz.zycfv.cn/gtvoepyatt.html

ruff format . && ruff check --fix .
来源：http://hz.sysykeji.top/gtawoebhqc.html

[U33] Py：打包发布
来源：http://hz.redwolf501.top/gtfxrskgog.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jlsjyb.cn/gtuyfnzqmg.html

[U34] Py：判断编码
来源：http://hz.jinghuilouyu.cn/gtihaootnp.html

chardet.detect(raw)
来源：http://hz.daxiang520.top/gtcturvvzk.html

[U35] Py：发送邮件
来源：http://hz.xinyue.icu/gtromyamcb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.aizwys.cn/gtgctxnjzx.html

[U36] Py：定时任务
来源：http://hz.yonumen.top/gterfdkuws.html

schedule.every(10).minutes.do(job)
来源：http://hz.52xcode.cn/gtvxyranom.html

[U37] Py：读写 Excel
来源：http://hz.yonumen.top/gtlfijsvww.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhengqikj.top/gtwclgmuve.html

[U38] Py：获取脚本所在目录
来源：http://hz.yangfankeji.com/gtrrdwmugi.html

Path(__file__).resolve().parent
来源：http://hz.shzxlz.cn/gtjcmasoni.html

[U39] Py：判断是否在交互环境
来源：http://hz.zdqjudy.top/gthyoksuzw.html

sys.stdout.isatty()
来源：http://hz.aizwys.cn/gtvxgcvsta.html

[U40] Py：打印到标准错误
来源：http://hz.yj20258888.top/gtdsmwmxge.html

print("err", file=sys.stderr)
来源：http://hz.chenjidiqi.icu/gtgdruspcy.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ppjwa.cn/gtjcdmtmoh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yanxiufei.cn/gtxjeyvhus.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.wangshuangyany.cn/gtyfrdhhys.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yvedp.cn/gtipehnste.html

[U43] PHP：声明命名空间
来源：http://hz.jinghuilouyu.cn/gtfufliynw.html

namespace App\Http;
来源：http://hz.xuetiantiany.cn/gtcwkqkrhh.html

[U44] PHP：开启严格类型
来源：http://hz.ivvv.top/gtsqenseit.html

declare(strict_types=1);
来源：http://hz.jinqigufen.top/gtuiqyxshl.html

[U45] PHP：类型声明与返回类型
来源：http://hz.wangshuangyany.cn/gtrogrbgxn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gttjbpeayq.html

[U46] PHP：可空类型
来源：http://hz.nanxinkj.top/gtfceipjuo.html

?string $name = null
来源：http://hz.wangshuangyany.cn/gtwfqwphsg.html

[U47] PHP：联合类型
来源：http://hz.nanxinkj.top/gtthhzedak.html

int|string $id
来源：http://hz.smart0.xyz/gtkpaypimc.html

[U48] PHP：纯枚举
来源：http://hz.jqgufenzy.top/gtgtjxfxhl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinqigfzy.top/gtvnauzlgx.html

[U49] PHP：只读属性
来源：http://hz.yonumen.top/gtlozffrxi.html

public readonly string $name
来源：http://hz.ydzc1.top/gtdxzhjear.html

[U50] PHP：构造器属性提升
来源：http://hz.yj202588.top/gtjgokvwsa.html

public function __construct(private int $id) {}
来源：http://hz.xziqi.cn/gtkqfdarec.html

[U51] PHP：数组解构
来源：http://hz.52xcode.cn/gtignmweie.html

[$a, $b] = $arr;
来源：http://hz.hnqzz.top/gtdapccafj.html

[U52] PHP：箭头函数
来源：http://hz.chenzaomai.com/gtcxyzxjwq.html

$double = fn($x) => $x * 2;
来源：http://hz.yj20258.top/gtvlwiyffw.html

[U53] PHP：空合并运算符
来源：http://hz.hnqzz.top/gtgjjopsup.html

$v = $a ?? $b ?? "default";
来源：http://hz.guowangkeji.top/gtknjasvol.html

[U54] PHP：空安全调用
来源：http://hz.ehwqpu.com/gttjqovred.html

$obj?->method()
来源：http://hz.zhaomingkeji.xyz/gtddwqkvjj.html

[U55] PHP：match 表达式
来源：http://hz.jyoumei.cn/gtchdvwscs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.daria6918.cn/gtvsnumclj.html

[U56] PHP：命名参数
来源：http://hz.guannengcc.top/gthqcplons.html

f(a: 1, b: 2)
来源：http://hz.zhengqikj.top/gtpzfnsgie.html

[U57] PHP：字符串插值
来源：http://hz.zhengqikj.top/gtrdqmcthk.html

"值: {$a}"
来源：http://hz.316326.xyz/gtchldfyty.html

[U58] PHP：数组三件套
来源：http://hz.xziqi.cn/gtnysromfj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jqgufenzy.top/gtnbrlocwd.html

[U59] PHP：自定义排序
来源：http://hz.hnxiangtu.top/gtoaokqxil.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.9152youxi.cn/gtouyaokgg.html

[U60] PHP：JSON 编解码
来源：http://hz.daria6918.cn/gtuuazcwis.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jqgufenzy.top/gtnuivhblh.html


<!-- 参考信息 -->