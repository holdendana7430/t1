代发 wailian999

#include <iostream>
来源：http://hz.chenlongwang.top/gtukbojtzc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.fzhhl.top/gtzpzcxtun.html

[S32] C++：字符串
来源：http://hz.yuanzhike.top/gtfbuuyuwg.html

std::string s = "hi";  s += "!";
来源：http://hz.ydzc1.top/gtnsohufih.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtkdhrmpef.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhixingplan.top/gtczwwzpip.html

[S34] C++：遍历 vector
来源：http://hz.zhijiandao.cn/gtcrignqkl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hongshengwenyu.top/gtimifbtio.html

[S35] C++：map
来源：http://hz.hongshengwenyu.top/gtwloarubo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.meibo888.top/gtvkrosmyr.html

[S36] C++：unordered_map
来源：http://hz.gaohongyu789.top/gtwhzhvrqh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.redwolf501.top/gtcigqhfsg.html

[S37] C++：set
来源：http://hz.smart0.xyz/gtmqpdpjdn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sxryk.cn/gtesnwnflx.html

[S38] C++：排序
来源：http://hz.dashuyun.cn/gtzgmhrcjb.html

std::sort(v.begin(), v.end());
来源：http://hz.hnqzz.top/gtqyxqfmlj.html

[S39] C++：自定义比较器排序
来源：http://hz.yongpay.top/gtucyiuqyo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hysaishi.cn/gtwwdmvglc.html

[S40] C++：查找元素
来源：http://hz.sysykeji.top/gtcfugdypu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuxming.cn/gtrfpbzxrg.html

[S41] C++：类与构造函数
来源：http://hz.52xcode.cn/gtqfrjvvqn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.feifeiyinyue.top/gtjqrocxpu.html

[S42] C++：继承与虚函数
来源：http://hz.yuxming.cn/gtgwdoxwja.html

class B : public Base { public: void f() override {} };
来源：http://hz.iojbl.cn/gtvfycqbnw.html

[S43] C++：智能指针
来源：http://hz.sweek.top/gtxngtozhn.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhaomingkeji.xyz/gthixyurfs.html

[S44] C++：引用传参
来源：http://hz.yuanzhike.top/gtzhavrdfw.html

void inc(int &x) { ++x; }
来源：http://hz.wangshuangyany.cn/gtbwnqlxqg.html

[S45] C++：lambda
来源：http://hz.feifeiyinyue.top/gtfsmogolh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yj20258.top/gtekewqeip.html

[S46] C++：函数模板
来源：http://hz.jlsjyb.cn/gtakmeqyso.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.vqdsnc.cn/gtwgsmaqfo.html

[S47] C++：结构化绑定遍历
来源：http://hz.aizwys.cn/gtwqsqqrrc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.c1oappe.top/gtbhtpbwmw.html

[S48] C++：逐行读文件
来源：http://hz.hnxiangtu.top/gtiezccmjs.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hywenlv.cn/gtafamyuum.html

while (std::getline(in, line)) { }
来源：http://hz.shangyingyoupin.top/gtgziherhs.html

[S49] C++：写文件
来源：http://hz.yueranfly.top/gtiggibeef.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sysykeji.top/gtadjiqjvz.html

[S50] C++：格式化数字
来源：http://hz.jinqigfzy.top/gttbtmyjml.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigufen.top/gtdjwxyjld.html

[S51] C++：显式类型转换
来源：http://hz.hfpthk.cn/gtujkatnno.html

static_cast<double>(a) / b
来源：http://hz.yongpay.top/gtqdzgbiws.html

[S52] C++：const 与 noexcept
来源：http://hz.52xcode.cn/gtotsdncvg.html

int size() const noexcept { return n_; }
来源：http://hz.zhixingplan.top/gtfuekfgiw.html

[S53] C++：移动语义
来源：http://hz.hysaishi.cn/gtesssnxin.html

std::vector<int> w = std::move(v);
来源：http://hz.hammf.cn/gtzcfhjijf.html

[S54] C++：异常处理
来源：http://hz.birdmap.top/gtltjsqcve.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jiagoushi.top/gtyflxugdo.html

[S55] C++：结构化绑定
来源：http://hz.zhijiandao.cn/gtrifxhocm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ywan-chungtsiang.top/gtghofdqmy.html

[S56] C++：optional
来源：http://hz.0kj1m.cn/gtruhalvoh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ywan-chungtsiang.top/gtrsfnxqed.html

[S57] C++：编译期常量
来源：http://hz.feifeiyinyue.top/gtrmbftmcn.html

constexpr int N = 10;
来源：http://hz.zhiwuduotai.top/gtyvrxbehm.html

[S58] C++：命名空间
来源：http://hz.yj20258.top/gtmkhwvfkg.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinqigufen.top/gtpyunakyi.html

[S59] C++：静态断言
来源：http://hz.hnqzz.top/gtpcrjnxce.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.mhx1999.top/gtrvmihcqo.html

[S60] C++：遍历并删除元素
来源：http://hz.vqdsnc.cn/gtrrcpgtnj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hongshengwenyu.top/gtpqixvjky.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gthkofpjkt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zycfv.cn/gtmmeeesah.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgxveboor.html

[T01] Kotlin：Hello World
来源：http://hz.hnxiangtu.top/gttkyhxfvx.html

println("Hello")
来源：http://hz.andypj.xyz/gthuwjojdi.html

[T02] Kotlin：变量
来源：http://hz.zhongyouzk.top/gtvnpqkoos.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangdashe.top/gtuvcmuhmk.html

[T03] Kotlin：字符串模板
来源：http://hz.316326.xyz/gtorggfvyc.html

"值: $b"
来源：http://hz.nwbrower.top/gthzcsnvbd.html

[T04] Kotlin：空安全
来源：http://hz.zhengqikj.top/gtetssprod.html

val n: String? = null;  n?.length
来源：http://hz.yj20258888.top/gtdpneznfa.html

[T05] Kotlin：when 表达式
来源：http://hz.cqqwz.cn/gtiwiwpxty.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.dashuyun.cn/gtbmlfehkk.html

[T06] Kotlin：集合映射
来源：http://hz.zhengqikj.top/gtqbchxncn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.kuanghao11.cn/gtzllrkxjh.html

[T07] Kotlin：集合过滤
来源：http://hz.nanxinkj.top/gtlfhgiove.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nanxinkj.top/gtzumkutvz.html

[T08] Kotlin：数据类
来源：http://hz.daria6918.cn/gtmwudqzaf.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgfzy.top/gtpxupwlbv.html

[T09] Kotlin：扩展函数
来源：http://hz.yj20258.top/gtmuhjvrfy.html

fun String.exclaim() = this + "!"
来源：http://hz.cheryme.top/gtoxdgvosf.html

[T10] Kotlin：默认参数
来源：http://hz.jinyuanbaomall.cn/gtcpbpbmxx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenlongwang.top/gtskkyotez.html

[T11] Kotlin：协程
来源：http://hz.hysaishi.cn/gtooaghhlr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jqgufenzy.top/gttmjflsno.html

[T12] Kotlin：解构声明
来源：http://hz.ydjk.org.cn/gtthaqygig.html

val (a, b) = Pair(1, 2)
来源：http://hz.yangfankeji.com/gtsftfgwjf.html

[T13] Kotlin：只读 Map
来源：http://hz.jyoumei.cn/gtbuiwqvul.html

val m = mapOf("a" to 1)
来源：http://hz.sufxvd.cn/gtwhgghbnm.html

[T14] Kotlin：循环
来源：http://hz.yangfankeji.com/gtrpldhlmt.html

for (i in 1..10) println(i)
来源：http://hz.tanke756.top/gtdjidpxex.html

[T15] Kotlin：接口
来源：http://hz.hnqzz.top/gtsvbiurkw.html

interface Shape { fun area(): Double }
来源：http://hz.xuetiantiany.cn/gtgseqmdxl.html

[T16] Swift：Hello World
来源：http://hz.pycfn.com/gtncidyrbi.html

print("Hello")
来源：http://hz.yongpay.top/gtuabjmuil.html

[T17] Swift：变量与常量
来源：http://hz.dianchejie.cn/gtndlpsaiq.html

var a = 1;  let b = 2
来源：http://hz.fzhhl.top/gtwavvtpsx.html

[T18] Swift：字符串插值
来源：http://hz.chenlongwang.top/gtydvdcerq.html

"值: \(b)"
来源：http://hz.gogol.net.cn/gtplahmpys.html

[T19] Swift：可选绑定
来源：http://hz.tian-w.cn/gtxgankbyq.html

if let n = opt { print(n) }
来源：http://hz.yj20258888.top/gtsundwcze.html

[T20] Swift：数组操作
来源：http://hz.fzhhl.top/gtyfrfhbur.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sysykeji.top/gtalnoscws.html

[T21] Swift：遍历
来源：http://hz.shanyushiyangkeji.top/gtttlbxprt.html

for x in a { print(x) }
来源：http://hz.cashguo.top/gtvgaszznu.html

[T22] Swift：字典
来源：http://hz.dashuyun.cn/gtyeimwmlo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cheryme.top/gtwtwdulxa.html

[T23] Swift：函数
来源：http://hz.zhaomingkeji.xyz/gtinhomngo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.pengpengdd.cyou/gtxdzfolxi.html

[T24] Swift：闭包
来源：http://hz.ybcxt.top/gtgikrhptg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jlsjyb.cn/gttqzcwidx.html

[T25] Swift：结构体
来源：http://hz.sysykeji.top/gtwdnrwkth.html

struct P { var x: Int }
来源：http://hz.fengsongda.top/gtstsipruh.html

[T26] Swift：类与重写
来源：http://hz.wangshuangyany.cn/gtnugaovvw.html

class A: Base { override func f() {} }
来源：http://hz.jinyuanbaomall.cn/gtqsecrbur.html

[T27] Swift：错误处理
来源：http://hz.daxiang520.top/gtxaopsmee.html

do { try f() } catch { print(error) }
来源：http://hz.zhongyouzk.top/gtxywzsrig.html

[T28] Swift：枚举
来源：http://hz.fengsongda.top/gtvlwhlzkk.html

enum Color { case red, green }
来源：http://hz.jyoumei.cn/gtdnlcufjo.html

[T29] Swift：guard 提前返回
来源：http://hz.svipenyu.cn/gtcuapdfyq.html

guard let x = opt else { return }
来源：http://hz.feifeiyinyue.top/gtrsxfsild.html

[T30] Swift：协议
来源：http://hz.jqgufenzy.top/gtkygmanbr.html

protocol Shape { func area() -> Double }
来源：http://hz.cqqwz.cn/gtgepvjkvh.html

[T31] Lua：Hello World
来源：http://hz.andypj.xyz/gthoommboc.html

print("Hello")
来源：http://hz.hnqzz.top/gtrbnxiasu.html

[T32] Lua：局部变量
来源：http://hz.xinyue.icu/gtbsrfuzxg.html

local a = 1
来源：http://hz.hnqzz.top/gteheemkmq.html

[T33] Lua：表（数组）
来源：http://hz.gaohongyu789.top/gtmlsxlgyb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinyuanbaomall.cn/gtniwvvnsq.html

[T34] Lua：遍历表
来源：http://hz.zhixingplan.top/gtlawlqozp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hfpthk.cn/gtqjkabdfw.html

[T35] Lua：字典表
来源：http://hz.ydzc1.top/gtjtdyzoqq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.daxiang520.top/gtwtfbtfqs.html

[T36] Lua：函数
来源：http://hz.zycfv.cn/gthsrvafpr.html

function add(a, b) return a + b end
来源：http://hz.meibo888.top/gtrvsifshw.html

[T37] Lua：字符串拼接
来源：http://hz.chenlongwang.top/gtonaehdfp.html

"a" .. "b"
来源：http://hz.jinqigfzy.top/gtsikjnuts.html

[T38] Lua：条件
来源：http://hz.zhijiandao.cn/gtlyuawldw.html

if x > 0 then print("正") end
来源：http://hz.hywenlv.cn/gtqkivcijz.html

[T39] Lua：模式匹配
来源：http://hz.yj20258.top/gtmyhzszww.html

string.find(s, "%d+")
来源：http://hz.redwolf501.top/gtsswkaazj.html

[T40] Lua：元表
来源：http://hz.jinghuilouyu.cn/gtjkfjomwl.html

setmetatable({}, { __index = base })
来源：http://hz.sysykeji.top/gtrpehnbcw.html

[T41] Perl：Hello World
来源：http://hz.zhengqikj.top/gtxfvcwunm.html

print "Hello\n";
来源：http://hz.shanyushiyangkeji.top/gtrqjnfhzf.html

[T42] Perl：变量类型
来源：http://hz.fengsongda.top/gtsjlufcnp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.meibo888.top/gthymthgfb.html

[T43] Perl：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtrrzizxqq.html

"值: $a"
来源：http://hz.zhixingplan.top/gtabwjpssu.html

[T44] Perl：条件
来源：http://hz.ydjk.org.cn/gtbgxbkpzq.html

if ($a > 0) { print "正"; }
来源：http://hz.snrcjt.cn/gtvclycsns.html

[T45] Perl：数组遍历
来源：http://hz.zhixingplan.top/gtpfuhptdv.html

for my $x (@arr) { print $x; }
来源：http://hz.cheryme.top/gtwttxverz.html

[T46] Perl：哈希操作
来源：http://hz.nwbrower.top/gtunxlkenr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhixingplan.top/gtcmgsusmm.html

[T47] Perl：正则捕获
来源：http://hz.ydjk.org.cn/gtozcvzttl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.redwolf501.top/gtpfbjvbiz.html

[T48] Perl：正则替换
来源：http://hz.pengpengdd.cyou/gtckunjidf.html

$s =~ s/old/new/g;
来源：http://hz.zhiwuduotai.top/gtmddzknnp.html

[T49] Perl：函数
来源：http://hz.ehwqpu.com/gteioxmtsf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.aibaodan.cn/gtxqsgecse.html

[T50] Perl：逐行读文件
来源：http://hz.hfpthk.cn/gtngsxstox.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hammf.cn/gtqosexcvm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hywenlv.cn/gtxqfdgujr.html

[T51] Scala：Hello World
来源：http://hz.9152youxi.cn/gtvipnbble.html

println("Hello")
来源：http://hz.chenjidiqi.icu/gtzjvysakt.html

[T52] Scala：变量
来源：http://hz.pengpengdd.cyou/gtpcljmvah.html

val a = 1;  var b = 2
来源：http://hz.shuidangran.top/gtxidqhzhp.html

[T53] Scala：字符串插值
来源：http://hz.c1oappe.top/gtipzyxqha.html

s"值: $b"
来源：http://hz.andypj.xyz/gtrcjwoiwb.html

[T54] Scala：集合映射
来源：http://hz.yj202588.top/gtontmisml.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jianghu66.top/gtdaicuemi.html

[T55] Scala：集合过滤
来源：http://hz.shanyushiyangkeji.top/gtlqfthrgf.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cucudq.cn/gtowtekuyl.html

[T56] Scala：样例类
来源：http://hz.jinghuilouyu.cn/gtpecupczb.html

case class User(name: String, age: Int)
来源：http://hz.svipenyu.cn/gtuyatbftj.html

[T57] Scala：模式匹配
来源：http://hz.sxryk.cn/gtcwnhidzo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yongpay.top/gtblsomjmi.html

[T58] Scala：函数定义
来源：http://hz.xinyue.icu/gtcmmouwsi.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jlsjyb.cn/gtfqddbwkr.html

[T59] Scala：循环
来源：http://hz.ivvv.top/gthdufmsax.html

for (i <- 1 to 10) println(i)
来源：http://hz.ydzc1.top/gtsnvbcnjf.html

[T60] Scala：折叠
来源：http://hz.yueranfly.top/gtstvbmtcx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xziqi.cn/gtxksetovc.html

================================================================================
来源：http://hz.iojbl.cn/gtkrrorvol.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.daria6918.cn/gtkbxzgzcj.html

================================================================================
来源：http://hz.havefunace.top/gtlkmttilg.html

[U01] Py：创建虚拟环境
来源：http://hz.xinyue.icu/gtktbkxkjm.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xziqi.cn/gtcmwxhrcs.html

[U02] Py：导出 / 安装依赖
来源：http://hz.aibaodan.cn/gtqkgpcmrc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.fzhhl.top/gtlrxhtvga.html

[U03] Py：加载 .env 配置
来源：http://hz.gzhubu.top/gtmkdnmakv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xuetiantiany.cn/gtikwsprqi.html

[U04] Py：变量调试打印
来源：http://hz.jiagoushi.top/gtxrcsvpie.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.fengsongda.top/gtczmpztwl.html

[U05] Py：列表去重且保序
来源：http://hz.jqgufenzy.top/gtcxolzhhk.html

list(dict.fromkeys(arr))
来源：http://hz.kuanghao11.cn/gtdawtcxuk.html

[U06] Py：合并两个字典
来源：http://hz.andypj.xyz/gtbuqcxqiw.html

{**a, **b}
来源：http://hz.daxiang520.top/gthjhzuref.html

[U07] Py：反转字典键值
来源：http://hz.iojbl.cn/gtbhvucdlb.html

{v: k for k, v in d.items()}
来源：http://hz.cqqwz.cn/gtulkbctsf.html

[U08] Py：展平二维列表
来源：http://hz.hysaishi.cn/gtoxolajra.html

[y for x in nested for y in x]
来源：http://hz.9152youxi.cn/gtnhfkzuck.html

[U09] Py：字典取最大值的键
来源：http://hz.redwolf501.top/gtthxvivil.html

max(d, key=d.get)
来源：http://hz.hammf.cn/gtetoiyiqu.html

[U10] Py：按值排序字典
来源：http://hz.zhoulong.xyz/gtjkojcckf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ppjwa.cn/gtyizwoyny.html

[U11] Py：生成器表达式
来源：http://hz.zhijiandao.cn/gtiaoluoni.html

(x * 2 for x in arr)
来源：http://hz.jinyuanbaomall.cn/gtpzzlunto.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.haohaochexian.top/gtluvebilx.html

Counter(arr).most_common(3)
来源：http://hz.hnxiangtu.top/gtlztykesl.html

[U13] Py：固定长度队列
来源：http://hz.feifeiyinyue.top/gtdnshmpbn.html

deque(maxlen=10)
来源：http://hz.cashguo.top/gtgvlstwpb.html

[U14] Py：分组收集到列表
来源：http://hz.sysykeji.top/gtxwdcacxy.html

defaultdict(list)
来源：http://hz.snrcjt.cn/gtzkqsaslt.html

[U15] Py：高精度计时
来源：http://hz.chenjidiqi.icu/gtkdelsoyi.html

t = time.perf_counter()
来源：http://hz.jlsjyb.cn/gtxcgklmww.html

[U16] Py：命令行参数解析
来源：http://hz.shuidangran.top/gtjzhmruxe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cdnleiting.top/gtdkrotyqb.html

[U17] Py：初始化日志
来源：http://hz.sweek.top/gtlgylunlm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yangfankeji.com/gtumohnobx.html

[U18] Py：预编译正则
来源：http://hz.havefunace.top/gteoffvjgx.html

pat = re.compile(r"\d+")
来源：http://hz.shangyingyoupin.top/gtjnoazvlp.html

[U19] Py：正则替换带回调
来源：http://hz.hywenlv.cn/gtvdfleurd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hysaishi.cn/gtinbbliai.html

[U20] Py：缓存函数结果
来源：http://hz.yj20258888.top/gtvmgkkheu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhijiandao.cn/gtvjjddtio.html

[U21] Py：自定义上下文管理器
来源：http://hz.jiagoushi.top/gtkupubtmr.html

@contextlib.contextmanager
来源：http://hz.cdnleiting.top/gtroalupzk.html

[U22] Py：矩阵转置
来源：http://hz.snrcjt.cn/gtlzjknpya.html

list(zip(*m))
来源：http://hz.yj20258888.top/gtbwgdlvab.html

[U23] Py：分块读取大文件
来源：http://hz.zycfv.cn/gtrfwtsmmj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.guowangkeji.top/gtqsldgvjn.html

[U24] Py：路径操作
来源：http://hz.jinyuanbaomall.cn/gtsxweizbb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gotoacloud.top/gtxhsvzlby.html

[U25] Py：CSV 按字典读
来源：http://hz.jinghuilouyu.cn/gtrothjnev.html

csv.DictReader(f)
来源：http://hz.nanxuanxn.top/gtotndgyqc.html

[U26] Py：并发下载
来源：http://hz.zhoulong.xyz/gtvoyyqrwq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.smart0.xyz/gtxwewlkzk.html

[U27] Py：异步 HTTP
来源：http://hz.zhaomingkeji.xyz/gtnrdrjbsj.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sweek.top/gtgregiiyg.html

[U28] Py：类型别名
来源：http://hz.ywan-chungtsiang.top/gtlcioqsyi.html

UserId = int
来源：http://hz.hysaishi.cn/gtdiclrmmy.html

[U29] Py：属性校验
来源：http://hz.cashguo.top/gtotijmzoe.html

@property 与 @x.setter 配合
来源：http://hz.yvedp.cn/gtoshybzyn.html

[U30] Py：数据类
来源：http://hz.haohaochexian.top/gtvknpktxg.html

@dataclass(slots=True)
来源：http://hz.hnqzz.top/gtpisodmbd.html

[U31] Py：单测
来源：http://hz.aibaodan.cn/gtlqvbclgr.html

python -m pytest -q
来源：http://hz.jqgfzy.top/gtilsicuyk.html

[U32] Py：代码格式化
来源：http://hz.daxiang520.top/gtauxmtaal.html

ruff format . && ruff check --fix .
来源：http://hz.sweek.top/gtcpjkxjay.html

[U33] Py：打包发布
来源：http://hz.hfpthk.cn/gtgamdfqaw.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ivvv.top/gtjuoxbfbj.html

[U34] Py：判断编码
来源：http://hz.xingfuxueyuan.xyz/gtzrigbomi.html

chardet.detect(raw)
来源：http://hz.chenlongwang.top/gthugtcuvb.html

[U35] Py：发送邮件
来源：http://hz.redwolf501.top/gtlsmuiptx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.sxryk.cn/gtthopvugo.html

[U36] Py：定时任务
来源：http://hz.andypj.xyz/gtopfumrsd.html

schedule.every(10).minutes.do(job)
来源：http://hz.yvedp.cn/gtwrksabqj.html

[U37] Py：读写 Excel
来源：http://hz.zhijiandao.cn/gtadrlgqaz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.guannengcc.top/gtpquftqpk.html

[U38] Py：获取脚本所在目录
来源：http://hz.ybcxt.top/gtxdazoplw.html

Path(__file__).resolve().parent
来源：http://hz.guannengcc.top/gtrohnrowk.html

[U39] Py：判断是否在交互环境
来源：http://hz.yvedp.cn/gtdzfzywcn.html

sys.stdout.isatty()
来源：http://hz.havefunace.top/gtaiijambr.html

[U40] Py：打印到标准错误
来源：http://hz.zhengqikj.top/gthorzbzse.html

print("err", file=sys.stderr)
来源：http://hz.gotoacloud.top/gtxzpkqgas.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.wangdashe.top/gtxtlzuetl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.gotoacloud.top/gtydmasmpg.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zycfv.cn/gtclbnksfe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinyuanbaomall.cn/gtgwlkgdgq.html

[U43] PHP：声明命名空间
来源：http://hz.guowangkeji.top/gtkmcyuzhl.html

namespace App\Http;
来源：http://hz.jyoumei.cn/gtxqbcreha.html

[U44] PHP：开启严格类型
来源：http://hz.tanke756.top/gtspbyvdsr.html

declare(strict_types=1);
来源：http://hz.sysykeji.top/gtnocigncr.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shuidangran.top/gtevfnwphv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gthecwpdji.html

[U46] PHP：可空类型
来源：http://hz.gaohongyu789.top/gtqtmzgeru.html

?string $name = null
来源：http://hz.iojbl.cn/gtvadcslsr.html

[U47] PHP：联合类型
来源：http://hz.birdmap.top/gthyanyzhg.html

int|string $id
来源：http://hz.xingfuxueyuan.xyz/gtagyacmao.html

[U48] PHP：纯枚举
来源：http://hz.haohaochexian.top/gtnmqbephd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ivvv.top/gtqkefflmu.html

[U49] PHP：只读属性
来源：http://hz.pycfn.com/gtfwwrdbwz.html

public readonly string $name
来源：http://hz.hfpthk.cn/gtnbsnohfp.html

[U50] PHP：构造器属性提升
来源：http://hz.ivvv.top/gtrnpezguv.html

public function __construct(private int $id) {}
来源：http://hz.fengsongda.top/gtlznybffn.html

[U51] PHP：数组解构
来源：http://hz.meibo888.top/gtraolasuv.html

[$a, $b] = $arr;
来源：http://hz.tian-w.cn/gtpdkhnian.html

[U52] PHP：箭头函数
来源：http://hz.cucudq.cn/gtgeoqmzkp.html

$double = fn($x) => $x * 2;
来源：http://hz.zhixingplan.top/gtjlojqoet.html

[U53] PHP：空合并运算符
来源：http://hz.jinqigfzy.top/gtgzcoofge.html

$v = $a ?? $b ?? "default";
来源：http://hz.jqgufenzy.top/gtzylfonaw.html

[U54] PHP：空安全调用
来源：http://hz.guowangkeji.top/gtacoiutot.html

$obj?->method()
来源：http://hz.yj20258888.top/gtehbkvqdz.html

[U55] PHP：match 表达式
来源：http://hz.tanke756.top/gtyfdfxmde.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhijiandao.cn/gtqogndgvw.html

[U56] PHP：命名参数
来源：http://hz.nwbrower.top/gtrkwdlyte.html

f(a: 1, b: 2)
来源：http://hz.jinqigufen.top/gtcpunalsg.html


<!-- 参考信息 -->