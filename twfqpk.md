代发 wailian999

#include <iostream>
来源：http://hz.zhongyouzk.top/gtdetqslya.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.dashuyun.cn/gtavzmttpb.html

[S32] C++：字符串
来源：http://hz.ydjk.org.cn/gtkvoytrsv.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangtech.top/gteuypmmiu.html

[S33] C++：vector 增删
来源：http://hz.chenjidiqi.icu/gtqmyayjcc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jyoumei.cn/gtcstqtpjm.html

[S34] C++：遍历 vector
来源：http://hz.hnxiangtu.top/gtefmuqhdc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jianghu66.top/gttyzvvrbb.html

[S35] C++：map
来源：http://hz.tianlin.xyz/gtpnkhuhcb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dashuyun.cn/gtnhejkzqe.html

[S36] C++：unordered_map
来源：http://hz.jqgfzy.top/gtfjhxamkb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gttmurbkne.html

[S37] C++：set
来源：http://hz.shuidangran.top/gtpqmdnfrd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhijiandao.cn/gtzkmosuyh.html

[S38] C++：排序
来源：http://hz.nwbrower.top/gtzzsnwerx.html

std::sort(v.begin(), v.end());
来源：http://hz.yvedp.cn/gtvgrkgxtd.html

[S39] C++：自定义比较器排序
来源：http://hz.jqgufenzy.top/gtwvzaqcdr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ivvv.top/gtwcxzuqda.html

[S40] C++：查找元素
来源：http://hz.jinqigfzy.top/gtwwyeeqbq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jqgfzy.top/gtrfgvnycf.html

[S41] C++：类与构造函数
来源：http://hz.shanyushiyangkeji.top/gtuxfvixlg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.smart0.xyz/gttrbuaydb.html

[S42] C++：继承与虚函数
来源：http://hz.cqqwz.cn/gtmpvxxwdo.html

class B : public Base { public: void f() override {} };
来源：http://hz.wangdashe.top/gtmwlysngq.html

[S43] C++：智能指针
来源：http://hz.tanke756.top/gtcpnqtocv.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnqzz.top/gtypmdfeao.html

[S44] C++：引用传参
来源：http://hz.nanxinkj.top/gtevgvdimw.html

void inc(int &x) { ++x; }
来源：http://hz.chenjidiqi.icu/gtnlcmbvbs.html

[S45] C++：lambda
来源：http://hz.aibaodan.cn/gtflxxfvcm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ywan-chungtsiang.top/gtmtluyitn.html

[S46] C++：函数模板
来源：http://hz.xziqi.cn/gtvshublra.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ydjk.org.cn/gtvmxlvsfn.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnxiangtu.top/gtaxqqeoai.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xuanzx.com/gtboximaba.html

[S48] C++：逐行读文件
来源：http://hz.yvedp.cn/gtrsfruxqi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.iojbl.cn/gtmsikqnyl.html

while (std::getline(in, line)) { }
来源：http://hz.aizwys.cn/gtjmpvdlay.html

[S49] C++：写文件
来源：http://hz.andypj.xyz/gtrwbspcus.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daxiang520.top/gtsiegutoq.html

[S50] C++：格式化数字
来源：http://hz.jiagoushi.top/gthvlvdwjp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.pycfn.com/gtztynlmtm.html

[S51] C++：显式类型转换
来源：http://hz.jinghuilouyu.cn/gtajqrsyoa.html

static_cast<double>(a) / b
来源：http://hz.chenjidiqi.icu/gtnqtwobfu.html

[S52] C++：const 与 noexcept
来源：http://hz.hnqzz.top/gtfojmhnlc.html

int size() const noexcept { return n_; }
来源：http://hz.ehwqpu.com/gtuxnitpjv.html

[S53] C++：移动语义
来源：http://hz.dianchejie.cn/gtdefjpkaa.html

std::vector<int> w = std::move(v);
来源：http://hz.daxiang520.top/gthsyfhbgf.html

[S54] C++：异常处理
来源：http://hz.zhengqikj.top/gtmupfngno.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.redwolf501.top/gtysodmqmr.html

[S55] C++：结构化绑定
来源：http://hz.shzxlz.cn/gtadqobxex.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shanyushiyangtech.top/gtqwuabkea.html

[S56] C++：optional
来源：http://hz.fzhhl.top/gtzigquyxe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.fengsongda.top/gtuwbvkhjv.html

[S57] C++：编译期常量
来源：http://hz.yonumen.top/gtbujodsxf.html

constexpr int N = 10;
来源：http://hz.nanxuanxn.top/gtbxlwyfmf.html

[S58] C++：命名空间
来源：http://hz.zycfv.cn/gtlugeavdo.html

namespace ns { int f() { return 1; } }
来源：http://hz.pycfn.com/gtljgghxpe.html

[S59] C++：静态断言
来源：http://hz.hongshengwenyu.top/gtsetoqpms.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xziqi.cn/gtjpymofza.html

[S60] C++：遍历并删除元素
来源：http://hz.ivvv.top/gtdbxbcdul.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.aizwys.cn/gtgifdqcyg.html

================================================================================
来源：http://hz.hywenlv.cn/gtxfvxlxhk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jiagoushi.top/gtksnopbhw.html

================================================================================
来源：http://hz.zhongyouzk.top/gtuubcmxnp.html

[T01] Kotlin：Hello World
来源：http://hz.aibaodan.cn/gtrzqwtqal.html

println("Hello")
来源：http://hz.sweek.top/gtvtekltry.html

[T02] Kotlin：变量
来源：http://hz.cqqwz.cn/gtqnoztifq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj20258.top/gtzbnutnud.html

[T03] Kotlin：字符串模板
来源：http://hz.yuanzhike.top/gtjxumcpey.html

"值: $b"
来源：http://hz.daxiang520.top/gtwktalguo.html

[T04] Kotlin：空安全
来源：http://hz.birdmap.top/gtrlpzwdkc.html

val n: String? = null;  n?.length
来源：http://hz.daxiang520.top/gtafdlnrqp.html

[T05] Kotlin：when 表达式
来源：http://hz.pycfn.com/gtenzsbycp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xylfe.cn/gtpgehhqdz.html

[T06] Kotlin：集合映射
来源：http://hz.hywenlv.cn/gthwaabnmi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.vqdsnc.cn/gtjxgnitdt.html

[T07] Kotlin：集合过滤
来源：http://hz.xuanzx.com/gtkrhjjujo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sysykeji.top/gtnuewwslo.html

[T08] Kotlin：数据类
来源：http://hz.guowangkeji.top/gtgflmlmwu.html

data class User(val name: String, val age: Int)
来源：http://hz.zhengqikj.top/gttoiqkfsi.html

[T09] Kotlin：扩展函数
来源：http://hz.jianghu66.top/gtsjmnbvrw.html

fun String.exclaim() = this + "!"
来源：http://hz.sufxvd.cn/gtvlsgmiuo.html

[T10] Kotlin：默认参数
来源：http://hz.sxryk.cn/gtokffivkw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhixingplan.top/gtlfbhkgfx.html

[T11] Kotlin：协程
来源：http://hz.fengsongda.top/gtbchcynrt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuxming.cn/gtcnawvwfp.html

[T12] Kotlin：解构声明
来源：http://hz.xinyue.icu/gtisperehl.html

val (a, b) = Pair(1, 2)
来源：http://hz.9152youxi.cn/gtxcgmoqfi.html

[T13] Kotlin：只读 Map
来源：http://hz.haohaochexian.top/gtmftdpfuh.html

val m = mapOf("a" to 1)
来源：http://hz.xylfe.cn/gtsccveeql.html

[T14] Kotlin：循环
来源：http://hz.tian-w.cn/gtyxtzlyag.html

for (i in 1..10) println(i)
来源：http://hz.svipenyu.cn/gtcgwuklyo.html

[T15] Kotlin：接口
来源：http://hz.yj20258888.top/gtrwtfokdn.html

interface Shape { fun area(): Double }
来源：http://hz.hnqzz.top/gtabaildaz.html

[T16] Swift：Hello World
来源：http://hz.nanxuanxn.top/gtdfphcxcq.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gtkpcnmlmy.html

[T17] Swift：变量与常量
来源：http://hz.ehwqpu.com/gtlyybjvao.html

var a = 1;  let b = 2
来源：http://hz.aizwys.cn/gtnzoudreo.html

[T18] Swift：字符串插值
来源：http://hz.chenzaomai.com/gtoflvqzcu.html

"值: \(b)"
来源：http://hz.cdnleiting.top/gtivywpzhu.html

[T19] Swift：可选绑定
来源：http://hz.ehwqpu.com/gtnhdtsfnc.html

if let n = opt { print(n) }
来源：http://hz.zhengqikj.top/gturinfnpu.html

[T20] Swift：数组操作
来源：http://hz.feifeiyinyue.top/gtkmusehqe.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ivvv.top/gtgiziwgkc.html

[T21] Swift：遍历
来源：http://hz.chenlongwang.top/gtouygjyvr.html

for x in a { print(x) }
来源：http://hz.cdnleiting.top/gtgcbztshx.html

[T22] Swift：字典
来源：http://hz.hnxiangtu.top/gtwrwoxjnd.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.havefunace.top/gtfxbqjyfm.html

[T23] Swift：函数
来源：http://hz.gzhubu.top/gtefioseak.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sufxvd.cn/gthnliwuac.html

[T24] Swift：闭包
来源：http://hz.ybcxt.top/gtaktypoqe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.smart0.xyz/gtpkolucts.html

[T25] Swift：结构体
来源：http://hz.bjfxy.top/gtembhwwrk.html

struct P { var x: Int }
来源：http://hz.wangshuangyany.cn/gtjggkrktn.html

[T26] Swift：类与重写
来源：http://hz.quarkkingdee.top/gtizmmegqs.html

class A: Base { override func f() {} }
来源：http://hz.gzhubu.top/gtmcojblux.html

[T27] Swift：错误处理
来源：http://hz.0kj1m.cn/gtuxdoutsw.html

do { try f() } catch { print(error) }
来源：http://hz.sxryk.cn/gtoplzrwbj.html

[T28] Swift：枚举
来源：http://hz.xingfuxueyuan.xyz/gtnudalaha.html

enum Color { case red, green }
来源：http://hz.vqdsnc.cn/gtevfceqrh.html

[T29] Swift：guard 提前返回
来源：http://hz.c1oappe.top/gtjhqebued.html

guard let x = opt else { return }
来源：http://hz.nanxinkj.top/gtrwtdvbad.html

[T30] Swift：协议
来源：http://hz.andypj.xyz/gtpztidyvv.html

protocol Shape { func area() -> Double }
来源：http://hz.jiagoushi.top/gtoveyamdu.html

[T31] Lua：Hello World
来源：http://hz.cucudq.cn/gtixunkdfg.html

print("Hello")
来源：http://hz.jinqigufen.top/gtqktnthot.html

[T32] Lua：局部变量
来源：http://hz.ydzc1.top/gtbelbcpuh.html

local a = 1
来源：http://hz.yongpay.top/gtmsgjuzpr.html

[T33] Lua：表（数组）
来源：http://hz.jianghu66.top/gtwmgjshoq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinyuanbaomall.cn/gthksjpkae.html

[T34] Lua：遍历表
来源：http://hz.yuanzhike.top/gtcxruidvr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.iojbl.cn/gtffcwfogd.html

[T35] Lua：字典表
来源：http://hz.xuetiantiany.cn/gtlxxplqsu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gogol.net.cn/gthlnanwun.html

[T36] Lua：函数
来源：http://hz.vqdsnc.cn/gtzmcihtgb.html

function add(a, b) return a + b end
来源：http://hz.iojbl.cn/gtndcedrfs.html

[T37] Lua：字符串拼接
来源：http://hz.dashuyun.cn/gthhutebvd.html

"a" .. "b"
来源：http://hz.chenzaomai.com/gtbyxuuogt.html

[T38] Lua：条件
来源：http://hz.haohaochexian.top/gtszjbjbxo.html

if x > 0 then print("正") end
来源：http://hz.chenzaomai.com/gtscihfbyr.html

[T39] Lua：模式匹配
来源：http://hz.hfpthk.cn/gtctaifluc.html

string.find(s, "%d+")
来源：http://hz.jianghu66.top/gtwwetqyff.html

[T40] Lua：元表
来源：http://hz.fzhhl.top/gtmytzrdpp.html

setmetatable({}, { __index = base })
来源：http://hz.chenjidiqi.icu/gtbdtzuujp.html

[T41] Perl：Hello World
来源：http://hz.pengpengdd.cyou/gtqucbibhc.html

print "Hello\n";
来源：http://hz.hammf.cn/gteinorvdz.html

[T42] Perl：变量类型
来源：http://hz.wangdashe.top/gtjlgsjqxg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jqgfzy.top/gtlkowxyir.html

[T43] Perl：字符串插值
来源：http://hz.yanxiufei.cn/gtduqqplrt.html

"值: $a"
来源：http://hz.quarkkingdee.top/gtuycjxgkx.html

[T44] Perl：条件
来源：http://hz.hnxiangtu.top/gtalkfizth.html

if ($a > 0) { print "正"; }
来源：http://hz.jqgfzy.top/gtdeaffjuk.html

[T45] Perl：数组遍历
来源：http://hz.nanxinkj.top/gtyuqaizen.html

for my $x (@arr) { print $x; }
来源：http://hz.yonumen.top/gtvojsfonr.html

[T46] Perl：哈希操作
来源：http://hz.zhijiandao.cn/gtjsbikrth.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhixingplan.top/gtodyuelfp.html

[T47] Perl：正则捕获
来源：http://hz.guowangkeji.top/gtjdhoqnxg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.tianlin.xyz/gtyusvtiyb.html

[T48] Perl：正则替换
来源：http://hz.guannengcc.top/gtkpwtvjif.html

$s =~ s/old/new/g;
来源：http://hz.gotoacloud.top/gthjtfobmr.html

[T49] Perl：函数
来源：http://hz.jianghu66.top/gthavaxbuo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenjidiqi.icu/gtoxmydvhh.html

[T50] Perl：逐行读文件
来源：http://hz.tanke756.top/gtuaivenur.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xinyue.icu/gtjlihtuio.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yj202588.top/gtgoikfpcd.html

[T51] Scala：Hello World
来源：http://hz.jlsjyb.cn/gtnxqwsznt.html

println("Hello")
来源：http://hz.zhijiandao.cn/gtymylyoil.html

[T52] Scala：变量
来源：http://hz.yj20258888.top/gtpsqpdenh.html

val a = 1;  var b = 2
来源：http://hz.yuanzhike.top/gtrsjzlede.html

[T53] Scala：字符串插值
来源：http://hz.sweek.top/gtqpvphkzz.html

s"值: $b"
来源：http://hz.cqqwz.cn/gtfyagxnld.html

[T54] Scala：集合映射
来源：http://hz.xziqi.cn/gtpsnmaojp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xuanzx.com/gtgyozaine.html

[T55] Scala：集合过滤
来源：http://hz.jinqigfzy.top/gtvakpmxhe.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shzxlz.cn/gthqnuecfj.html

[T56] Scala：样例类
来源：http://hz.yj20258888.top/gtodatpyga.html

case class User(name: String, age: Int)
来源：http://hz.jinqigufen.top/gtmenlmzzn.html

[T57] Scala：模式匹配
来源：http://hz.snrcjt.cn/gtvwhzqqmm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shzxlz.cn/gtronyuvob.html

[T58] Scala：函数定义
来源：http://hz.jinqigufen.top/gtxhjtmjyj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sufxvd.cn/gtlqgtdhws.html

[T59] Scala：循环
来源：http://hz.shuidangran.top/gtbqanpvoa.html

for (i <- 1 to 10) println(i)
来源：http://hz.gzhubu.top/gtojreqflq.html

[T60] Scala：折叠
来源：http://hz.jlsjyb.cn/gthfpzegvp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shzxlz.cn/gtepapcwyu.html

================================================================================
来源：http://hz.cqqwz.cn/gtbmeaowsu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.vqdsnc.cn/gtqlfctkmd.html

================================================================================
来源：http://hz.yuanzhike.top/gtkopmkvqb.html

[U01] Py：创建虚拟环境
来源：http://hz.ivvv.top/gttzmlledc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.daria6918.cn/gtqdqktgnv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.nanxinkj.top/gtxdcjfxdu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zdqjudy.top/gtrnbqgtmc.html

[U03] Py：加载 .env 配置
来源：http://hz.aibaodan.cn/gtreiidwao.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yonumen.top/gtlbqkcveq.html

[U04] Py：变量调试打印
来源：http://hz.xinyue.icu/gtnpoxmree.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.haohaochexian.top/gterclvzvj.html

[U05] Py：列表去重且保序
来源：http://hz.hywenlv.cn/gtfumcgqyl.html

list(dict.fromkeys(arr))
来源：http://hz.jinyuanbaomall.cn/gtljnclgcd.html

[U06] Py：合并两个字典
来源：http://hz.xziqi.cn/gtibjgznqd.html

{**a, **b}
来源：http://hz.wangshuangyany.cn/gtetdflfxt.html

[U07] Py：反转字典键值
来源：http://hz.xinyue.icu/gtezfxrwmz.html

{v: k for k, v in d.items()}
来源：http://hz.sufxvd.cn/gtderrgong.html

[U08] Py：展平二维列表
来源：http://hz.fzhhl.top/gtwnumskba.html

[y for x in nested for y in x]
来源：http://hz.jianghu66.top/gtvhjxdszs.html

[U09] Py：字典取最大值的键
来源：http://hz.shanyushiyangtech.top/gthsvhfpjt.html

max(d, key=d.get)
来源：http://hz.haohaochexian.top/gtxvqphkqg.html

[U10] Py：按值排序字典
来源：http://hz.jqgufenzy.top/gtlybiexbd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.guannengcc.top/gtnthwxolb.html

[U11] Py：生成器表达式
来源：http://hz.daria6918.cn/gtmpeokwre.html

(x * 2 for x in arr)
来源：http://hz.hammf.cn/gtrjxjfarw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yuxming.cn/gthqbrumsu.html

Counter(arr).most_common(3)
来源：http://hz.iojbl.cn/gtohtvdnnc.html

[U13] Py：固定长度队列
来源：http://hz.gogol.net.cn/gtlpfyxdtj.html

deque(maxlen=10)
来源：http://hz.zhiwuduotai.top/gtqfsurqeb.html

[U14] Py：分组收集到列表
来源：http://hz.daria6918.cn/gtewdyexri.html

defaultdict(list)
来源：http://hz.xylfe.cn/gtbdgmvpfr.html

[U15] Py：高精度计时
来源：http://hz.tianlin.xyz/gtrlfoldgk.html

t = time.perf_counter()
来源：http://hz.zycfv.cn/gtsstooorj.html

[U16] Py：命令行参数解析
来源：http://hz.vqdsnc.cn/gthnywdhue.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinqigufen.top/gtnvjxxdnm.html

[U17] Py：初始化日志
来源：http://hz.sysykeji.top/gtejbqyllq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhiwuduotai.top/gtorqolxwe.html

[U18] Py：预编译正则
来源：http://hz.sxryk.cn/gttnjqyvde.html

pat = re.compile(r"\d+")
来源：http://hz.jinghuilouyu.cn/gttsrcwgnj.html

[U19] Py：正则替换带回调
来源：http://hz.shangyingyoupin.top/gtzlxuytmz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.tanke756.top/gtkvnkaqrs.html

[U20] Py：缓存函数结果
来源：http://hz.pengpengdd.cyou/gtdviiwwdp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jiagoushi.top/gtpagwpndb.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhongyouzk.top/gtnwprcrho.html

@contextlib.contextmanager
来源：http://hz.shanyushiyangkeji.top/gtfcvbdzhs.html

[U22] Py：矩阵转置
来源：http://hz.gogol.net.cn/gtkmuutats.html

list(zip(*m))
来源：http://hz.zhiwuduotai.top/gtvjoqphke.html

[U23] Py：分块读取大文件
来源：http://hz.tanke756.top/gtaytpqrnc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cheryme.top/gtlsvbpwpo.html

[U24] Py：路径操作
来源：http://hz.hongshengwenyu.top/gtsgiraiui.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yj202588.top/gtdzjiinia.html

[U25] Py：CSV 按字典读
来源：http://hz.yuxming.cn/gtavbabtol.html

csv.DictReader(f)
来源：http://hz.dianchejie.cn/gtizxcirlh.html

[U26] Py：并发下载
来源：http://hz.yangfankeji.com/gtnsrpqfno.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.aizwys.cn/gtjeyxlvrr.html

[U27] Py：异步 HTTP
来源：http://hz.aibaodan.cn/gthufvnbhl.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.dianchejie.cn/gtnshktzjy.html

[U28] Py：类型别名
来源：http://hz.wangshuangyany.cn/gtzxrzmlzg.html

UserId = int
来源：http://hz.ppjwa.cn/gtqgfbqaik.html

[U29] Py：属性校验
来源：http://hz.zhoulong.xyz/gtjaeaxmgx.html

@property 与 @x.setter 配合
来源：http://hz.yj20258.top/gttlaoxveb.html

[U30] Py：数据类
来源：http://hz.nanxuanxn.top/gtzuxnzzgu.html

@dataclass(slots=True)
来源：http://hz.c1oappe.top/gtmznxqmlz.html

[U31] Py：单测
来源：http://hz.9152youxi.cn/gtkspqckxt.html

python -m pytest -q
来源：http://hz.xuetiantiany.cn/gtfcbvspkt.html

[U32] Py：代码格式化
来源：http://hz.smart0.xyz/gtizmgevty.html

ruff format . && ruff check --fix .
来源：http://hz.chenjidiqi.icu/gtdvsiylbg.html

[U33] Py：打包发布
来源：http://hz.aibaodan.cn/gtpeqeznlz.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jinqigufen.top/gtfayapvhe.html

[U34] Py：判断编码
来源：http://hz.shzxlz.cn/gtfpvpsjob.html

chardet.detect(raw)
来源：http://hz.pengpengdd.cyou/gtwchcbyow.html

[U35] Py：发送邮件
来源：http://hz.yuanzhike.top/gthtbxknao.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.pengpengdd.cyou/gtjtnpevfs.html

[U36] Py：定时任务
来源：http://hz.yonumen.top/gtcmwxgzaz.html

schedule.every(10).minutes.do(job)
来源：http://hz.yuanzhike.top/gtcnocomew.html

[U37] Py：读写 Excel
来源：http://hz.fzhhl.top/gtujfodfry.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.vqdsnc.cn/gtvdzacorq.html

[U38] Py：获取脚本所在目录
来源：http://hz.gotoacloud.top/gteddwjjai.html

Path(__file__).resolve().parent
来源：http://hz.yuanzhike.top/gtimtdakid.html

[U39] Py：判断是否在交互环境
来源：http://hz.daria6918.cn/gtededhtfn.html

sys.stdout.isatty()
来源：http://hz.316326.xyz/gtiichkrmd.html

[U40] Py：打印到标准错误
来源：http://hz.yj20258.top/gtxngyyehy.html

print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gthyysqfzo.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.wangdashe.top/gtjjxbnrjg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.iojbl.cn/gtjiwpohmp.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xylfe.cn/gtlhokofjn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.tianlin.xyz/gtjwzrrvvu.html

[U43] PHP：声明命名空间
来源：http://hz.fengsongda.top/gtyoagzxxa.html

namespace App\Http;
来源：http://hz.redwolf501.top/gtmqcljygu.html

[U44] PHP：开启严格类型
来源：http://hz.jqgufenzy.top/gtppaqbkah.html

declare(strict_types=1);
来源：http://hz.jinqigfzy.top/gtzzjrbqbw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.gogol.net.cn/gtveuodwve.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.snrcjt.cn/gtqfshzmno.html

[U46] PHP：可空类型
来源：http://hz.quarkkingdee.top/gtvasxcrob.html

?string $name = null
来源：http://hz.pycfn.com/gteosuvqjb.html

[U47] PHP：联合类型
来源：http://hz.sysykeji.top/gtahdqzdvp.html

int|string $id
来源：http://hz.hongshengwenyu.top/gtrpxghywg.html

[U48] PHP：纯枚举
来源：http://hz.chenlongwang.top/gthphafzei.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.chenzaomai.com/gtkdpdihjs.html

[U49] PHP：只读属性
来源：http://hz.jqgufenzy.top/gtsbknlkoh.html

public readonly string $name
来源：http://hz.hammf.cn/gtnqzheymj.html

[U50] PHP：构造器属性提升
来源：http://hz.xziqi.cn/gtgcasurbp.html

public function __construct(private int $id) {}
来源：http://hz.zhoulong.xyz/gtdylofrpi.html

[U51] PHP：数组解构
来源：http://hz.ehwqpu.com/gtgleohkux.html

[$a, $b] = $arr;
来源：http://hz.andypj.xyz/gtmdulqzjd.html

[U52] PHP：箭头函数
来源：http://hz.sxryk.cn/gtasdulkfn.html

$double = fn($x) => $x * 2;
来源：http://hz.pycfn.com/gtnlgcefwg.html

[U53] PHP：空合并运算符
来源：http://hz.xuetiantiany.cn/gtgnlweafy.html

$v = $a ?? $b ?? "default";
来源：http://hz.chenzaomai.com/gtupipmztz.html

[U54] PHP：空安全调用
来源：http://hz.cqqwz.cn/gtjdfmnfnr.html

$obj?->method()
来源：http://hz.jqgufenzy.top/gtbhvrakzn.html

[U55] PHP：match 表达式
来源：http://hz.nanxuanxn.top/gtueagthok.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.52xcode.cn/gtcondjibm.html

[U56] PHP：命名参数
来源：http://hz.sweek.top/gtnahcbegg.html

f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtlfjhybhd.html


<!-- 参考信息 -->