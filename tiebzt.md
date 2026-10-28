代发 wailian999

[S37] C++：set
来源：http://hz.cqqwz.cn/gtrumoyixa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fengsongda.top/gtzhhwpfjl.html

[S38] C++：排序
来源：http://hz.ybcxt.top/gtnnzaijhw.html

std::sort(v.begin(), v.end());
来源：http://hz.zhiwuduotai.top/gtrzlbafia.html

[S39] C++：自定义比较器排序
来源：http://hz.iojbl.cn/gtfceftoqr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xziqi.cn/gtqotdchuo.html

[S40] C++：查找元素
来源：http://hz.tanke756.top/gtmetdrjgr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenlongwang.top/gtscpfpbbo.html

[S41] C++：类与构造函数
来源：http://hz.nanxuanxn.top/gtuakavbvn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.quarkkingdee.top/gtxctotlfj.html

[S42] C++：继承与虚函数
来源：http://hz.yangfankeji.com/gtwuofyyrs.html

class B : public Base { public: void f() override {} };
来源：http://hz.andypj.xyz/gtmekiznne.html

[S43] C++：智能指针
来源：http://hz.shanyushiyangtech.top/gtwxlyykzc.html

auto p = std::make_unique<int>(5);
来源：http://hz.ywan-chungtsiang.top/gtlclhcirf.html

[S44] C++：引用传参
来源：http://hz.cashguo.top/gtlcaxiimr.html

void inc(int &x) { ++x; }
来源：http://hz.gogol.net.cn/gtutndxfcr.html

[S45] C++：lambda
来源：http://hz.zdqjudy.top/gtncyttlgh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aizwys.cn/gtukhtjwwy.html

[S46] C++：函数模板
来源：http://hz.havefunace.top/gtuwbkiouz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hfpthk.cn/gteoosxmjf.html

[S47] C++：结构化绑定遍历
来源：http://hz.yangfankeji.com/gtbnsohxob.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yongpay.top/gtueiwmezq.html

[S48] C++：逐行读文件
来源：http://hz.hammf.cn/gtdwubgxnv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydjk.org.cn/gtdmtykwxo.html

while (std::getline(in, line)) { }
来源：http://hz.jqgfzy.top/gtarrcnmlr.html

[S49] C++：写文件
来源：http://hz.yuxming.cn/gtuxpcsknt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.meibo888.top/gtycnweezh.html

[S50] C++：格式化数字
来源：http://hz.yj202588.top/gtpoiqxxdb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ivvv.top/gtrnpqmysi.html

[S51] C++：显式类型转换
来源：http://hz.sweek.top/gtgkuojscl.html

static_cast<double>(a) / b
来源：http://hz.zhaomingkeji.xyz/gtnvkpjydh.html

[S52] C++：const 与 noexcept
来源：http://hz.jinghuilouyu.cn/gticfuxwur.html

int size() const noexcept { return n_; }
来源：http://hz.aibaodan.cn/gtjhmqmjiy.html

[S53] C++：移动语义
来源：http://hz.shangyingyoupin.top/gtkzvlxxmb.html

std::vector<int> w = std::move(v);
来源：http://hz.meibo888.top/gtpebiqodh.html

[S54] C++：异常处理
来源：http://hz.wangdashe.top/gtywygerle.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zycfv.cn/gthfumbtvd.html

[S55] C++：结构化绑定
来源：http://hz.mhx1999.top/gtrkhhgxia.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ivvv.top/gthlugsvje.html

[S56] C++：optional
来源：http://hz.daxiang520.top/gtbhlsspwt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinghuilouyu.cn/gtcbjylpfy.html

[S57] C++：编译期常量
来源：http://hz.smart0.xyz/gtlvfxlwdz.html

constexpr int N = 10;
来源：http://hz.yj202588.top/gtaxmsfutt.html

[S58] C++：命名空间
来源：http://hz.smart0.xyz/gtcircykfv.html

namespace ns { int f() { return 1; } }
来源：http://hz.xziqi.cn/gtntjsexhp.html

[S59] C++：静态断言
来源：http://hz.hongshengwenyu.top/gtkkmcfcns.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fzhhl.top/gtpnhyozqz.html

[S60] C++：遍历并删除元素
来源：http://hz.ppjwa.cn/gtzrhocwzc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhongyouzk.top/gtvsfmfxja.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtudoqajhr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuanzhike.top/gtujqycjyz.html

================================================================================
来源：http://hz.xuanzx.com/gtnrdqyriv.html

[T01] Kotlin：Hello World
来源：http://hz.shzxlz.cn/gtatpybtdt.html

println("Hello")
来源：http://hz.bjfxy.top/gtsaeqqgad.html

[T02] Kotlin：变量
来源：http://hz.pengpengdd.cyou/gtqgvfocvy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ybcxt.top/gtostaviuj.html

[T03] Kotlin：字符串模板
来源：http://hz.andypj.xyz/gteejimwug.html

"值: $b"
来源：http://hz.meibo888.top/gtwkyzwaqd.html

[T04] Kotlin：空安全
来源：http://hz.fzhhl.top/gtokgeacta.html

val n: String? = null;  n?.length
来源：http://hz.ivvv.top/gtqtzhjyrd.html

[T05] Kotlin：when 表达式
来源：http://hz.cucudq.cn/gturjbsoyk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tian-w.cn/gtvsgknnxv.html

[T06] Kotlin：集合映射
来源：http://hz.jqgufenzy.top/gtphkkaoie.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gotoacloud.top/gthjezlbak.html

[T07] Kotlin：集合过滤
来源：http://hz.dianchejie.cn/gtlklivoto.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.quarkkingdee.top/gtajuznqzw.html

[T08] Kotlin：数据类
来源：http://hz.yj20258.top/gtbbprojdu.html

data class User(val name: String, val age: Int)
来源：http://hz.snrcjt.cn/gtawvfntjh.html

[T09] Kotlin：扩展函数
来源：http://hz.hysaishi.cn/gtqscjxnga.html

fun String.exclaim() = this + "!"
来源：http://hz.xinyue.icu/gtnjrgufou.html

[T10] Kotlin：默认参数
来源：http://hz.daxiang520.top/gteewlwtzd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.haohaochexian.top/gtiywqnosf.html

[T11] Kotlin：协程
来源：http://hz.dianchejie.cn/gtfmerfihr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhongyouzk.top/gtgzhpnigk.html

[T12] Kotlin：解构声明
来源：http://hz.zhoulong.xyz/gtkqzlhxdp.html

val (a, b) = Pair(1, 2)
来源：http://hz.sweek.top/gtqsdyvtqx.html

[T13] Kotlin：只读 Map
来源：http://hz.ywan-chungtsiang.top/gteflbpkgv.html

val m = mapOf("a" to 1)
来源：http://hz.zhiwuduotai.top/gtgxgyckat.html

[T14] Kotlin：循环
来源：http://hz.havefunace.top/gtgyqtlyrv.html

for (i in 1..10) println(i)
来源：http://hz.xuetiantiany.cn/gtxrztonpn.html

[T15] Kotlin：接口
来源：http://hz.nanxuanxn.top/gtmdbudozj.html

interface Shape { fun area(): Double }
来源：http://hz.aibaodan.cn/gtkwgetrey.html

[T16] Swift：Hello World
来源：http://hz.hongshengwenyu.top/gtngwaczjm.html

print("Hello")
来源：http://hz.zhijiandao.cn/gtzhtytvua.html

[T17] Swift：变量与常量
来源：http://hz.yongpay.top/gtormdppvm.html

var a = 1;  let b = 2
来源：http://hz.sufxvd.cn/gtelmwrifj.html

[T18] Swift：字符串插值
来源：http://hz.zdqjudy.top/gtqcpgwrln.html

"值: \(b)"
来源：http://hz.ydjk.org.cn/gtbafuhjte.html

[T19] Swift：可选绑定
来源：http://hz.jqgufenzy.top/gtqaeoczfg.html

if let n = opt { print(n) }
来源：http://hz.hnxiangtu.top/gtjkpottif.html

[T20] Swift：数组操作
来源：http://hz.jyoumei.cn/gtjvomzbrx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daxiang520.top/gtcsnxhkqq.html

[T21] Swift：遍历
来源：http://hz.yueranfly.top/gtkraweerf.html

for x in a { print(x) }
来源：http://hz.jlsjyb.cn/gtcqluuopa.html

[T22] Swift：字典
来源：http://hz.yanxiufei.cn/gtehtnooeg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.mhx1999.top/gtcpfnhzez.html

[T23] Swift：函数
来源：http://hz.xylfe.cn/gtagrwnbiu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.vqdsnc.cn/gtwrzqbpab.html

[T24] Swift：闭包
来源：http://hz.0kj1m.cn/gtuvcrisej.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gzhubu.top/gtjmwlqfjf.html

[T25] Swift：结构体
来源：http://hz.xuetiantiany.cn/gtczmehkih.html

struct P { var x: Int }
来源：http://hz.c1oappe.top/gtrbnlmxtj.html

[T26] Swift：类与重写
来源：http://hz.yvedp.cn/gtfwjgptuj.html

class A: Base { override func f() {} }
来源：http://hz.shanyushiyangtech.top/gtwkbblikx.html

[T27] Swift：错误处理
来源：http://hz.cashguo.top/gtonxjvvhy.html

do { try f() } catch { print(error) }
来源：http://hz.ydzc1.top/gtwwlxeixg.html

[T28] Swift：枚举
来源：http://hz.316326.xyz/gtxznhbuce.html

enum Color { case red, green }
来源：http://hz.hongshengwenyu.top/gtlnovtcmx.html

[T29] Swift：guard 提前返回
来源：http://hz.hnqzz.top/gtqzybkopp.html

guard let x = opt else { return }
来源：http://hz.chenzaomai.com/gteizhlvge.html

[T30] Swift：协议
来源：http://hz.tianlin.xyz/gtsmgimqkh.html

protocol Shape { func area() -> Double }
来源：http://hz.iojbl.cn/gthxdpjqkq.html

[T31] Lua：Hello World
来源：http://hz.yj20258888.top/gtrekgazzc.html

print("Hello")
来源：http://hz.tanke756.top/gtcczvyblm.html

[T32] Lua：局部变量
来源：http://hz.xuanzx.com/gtiueugsgp.html

local a = 1
来源：http://hz.fzhhl.top/gtzxduzkvn.html

[T33] Lua：表（数组）
来源：http://hz.tanke756.top/gtwfhtsyrk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.9152youxi.cn/gttolonvmu.html

[T34] Lua：遍历表
来源：http://hz.jinghuilouyu.cn/gtwokdpkyn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cucudq.cn/gtzpejoizq.html

[T35] Lua：字典表
来源：http://hz.sufxvd.cn/gtztwdfoaw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj202588.top/gtwhuueiin.html

[T36] Lua：函数
来源：http://hz.gotoacloud.top/gtevdiikkm.html

function add(a, b) return a + b end
来源：http://hz.aizwys.cn/gtrjkoftur.html

[T37] Lua：字符串拼接
来源：http://hz.wangshuangyany.cn/gtxxreuiwt.html

"a" .. "b"
来源：http://hz.meibo888.top/gtrybpvtph.html

[T38] Lua：条件
来源：http://hz.yj202588.top/gthlpfkfqc.html

if x > 0 then print("正") end
来源：http://hz.gaohongyu789.top/gtfbhoewsd.html

[T39] Lua：模式匹配
来源：http://hz.fengsongda.top/gtoxsyrmty.html

string.find(s, "%d+")
来源：http://hz.daxiang520.top/gtaubahxyc.html

[T40] Lua：元表
来源：http://hz.yj202588.top/gtkiqzsjhu.html

setmetatable({}, { __index = base })
来源：http://hz.hammf.cn/gtirlskfap.html

[T41] Perl：Hello World
来源：http://hz.gaohongyu789.top/gtefdywaxs.html

print "Hello\n";
来源：http://hz.xinyue.icu/gtvhftaors.html

[T42] Perl：变量类型
来源：http://hz.yj20258.top/gtzntrrprj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yanxiufei.cn/gtyxtubyyq.html

[T43] Perl：字符串插值
来源：http://hz.52xcode.cn/gtqkpdjqfc.html

"值: $a"
来源：http://hz.jinqigufen.top/gtjaqlirav.html

[T44] Perl：条件
来源：http://hz.cucudq.cn/gtmstxcsfo.html

if ($a > 0) { print "正"; }
来源：http://hz.c1oappe.top/gtumgqwlob.html

[T45] Perl：数组遍历
来源：http://hz.yangfankeji.com/gtsjottipm.html

for my $x (@arr) { print $x; }
来源：http://hz.yj202588.top/gttcdsbpol.html

[T46] Perl：哈希操作
来源：http://hz.zhiwuduotai.top/gtvddqncip.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zycfv.cn/gtfyiyehbn.html

[T47] Perl：正则捕获
来源：http://hz.xinyue.icu/gtbrzbuxxh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cucudq.cn/gtbdihellt.html

[T48] Perl：正则替换
来源：http://hz.dashuyun.cn/gtupaaqefs.html

$s =~ s/old/new/g;
来源：http://hz.xziqi.cn/gtxtunuxlx.html

[T49] Perl：函数
来源：http://hz.zhijiandao.cn/gtypbtpmzw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhixingplan.top/gtvmagznsl.html

[T50] Perl：逐行读文件
来源：http://hz.snrcjt.cn/gtcalvxnpx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.shzxlz.cn/gtuhtwsqpm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yj20258.top/gtuqohpstq.html

[T51] Scala：Hello World
来源：http://hz.cqqwz.cn/gtfhowfnhn.html

println("Hello")
来源：http://hz.sufxvd.cn/gtzchpxodb.html

[T52] Scala：变量
来源：http://hz.wangdashe.top/gtdtnxnmpl.html

val a = 1;  var b = 2
来源：http://hz.sxryk.cn/gtevzirsxd.html

[T53] Scala：字符串插值
来源：http://hz.jlsjyb.cn/gtdmbkyknz.html

s"值: $b"
来源：http://hz.zhoulong.xyz/gthusyvaru.html

[T54] Scala：集合映射
来源：http://hz.ivvv.top/gthdhwqbim.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shzxlz.cn/gtrvlsjxwg.html

[T55] Scala：集合过滤
来源：http://hz.gaohongyu789.top/gtuttnjqud.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xylfe.cn/gtuhwatiqb.html

[T56] Scala：样例类
来源：http://hz.yuxming.cn/gtutlmiulz.html

case class User(name: String, age: Int)
来源：http://hz.havefunace.top/gtjuplukpc.html

[T57] Scala：模式匹配
来源：http://hz.cashguo.top/gtmkjvkumn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinyuanbaomall.cn/gtujviifom.html

[T58] Scala：函数定义
来源：http://hz.xziqi.cn/gtvsddtbfr.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.birdmap.top/gtlwqoewsj.html

[T59] Scala：循环
来源：http://hz.jqgufenzy.top/gtsllelydf.html

for (i <- 1 to 10) println(i)
来源：http://hz.guannengcc.top/gtxecpakmh.html

[T60] Scala：折叠
来源：http://hz.jianghu66.top/gtkporlqoh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xuanzx.com/gtimgbajbd.html

================================================================================
来源：http://hz.xziqi.cn/gtgdtosgps.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnqzz.top/gthucphzvw.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqjcyndau.html

[U01] Py：创建虚拟环境
来源：http://hz.kuanghao11.cn/gtzfxxkrnd.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.andypj.xyz/gtcgkxaaha.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenlongwang.top/gtqmwmjcup.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.c1oappe.top/gtidsmeatm.html

[U03] Py：加载 .env 配置
来源：http://hz.tanke756.top/gtqnbnzffa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ybcxt.top/gtlkjbquom.html

[U04] Py：变量调试打印
来源：http://hz.ppjwa.cn/gtnlahdcqn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.52xcode.cn/gtnrsmeaml.html

[U05] Py：列表去重且保序
来源：http://hz.hfpthk.cn/gtnodiyotc.html

list(dict.fromkeys(arr))
来源：http://hz.havefunace.top/gtfocfttnd.html

[U06] Py：合并两个字典
来源：http://hz.fzhhl.top/gtifyzkoni.html

{**a, **b}
来源：http://hz.aizwys.cn/gtgnfzxyic.html

[U07] Py：反转字典键值
来源：http://hz.jiagoushi.top/gtkqggivgc.html

{v: k for k, v in d.items()}
来源：http://hz.hysaishi.cn/gtgrraefty.html

[U08] Py：展平二维列表
来源：http://hz.guowangkeji.top/gtuxgxmpfn.html

[y for x in nested for y in x]
来源：http://hz.chenlongwang.top/gtinvcnrto.html

[U09] Py：字典取最大值的键
来源：http://hz.iojbl.cn/gtcnyciwpw.html

max(d, key=d.get)
来源：http://hz.yangfankeji.com/gtsvbguuuy.html

[U10] Py：按值排序字典
来源：http://hz.nwbrower.top/gtyfsgpzso.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.chenlongwang.top/gtsaamezed.html

[U11] Py：生成器表达式
来源：http://hz.ywan-chungtsiang.top/gtizzjgmhy.html

(x * 2 for x in arr)
来源：http://hz.yonumen.top/gtykmuxuzp.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yueranfly.top/gtlotzqzwx.html

Counter(arr).most_common(3)
来源：http://hz.daxiang520.top/gtfdmelpws.html

[U13] Py：固定长度队列
来源：http://hz.yvedp.cn/gtdegosida.html

deque(maxlen=10)
来源：http://hz.hnxiangtu.top/gtbhvglils.html

[U14] Py：分组收集到列表
来源：http://hz.cucudq.cn/gtehmfysre.html

defaultdict(list)
来源：http://hz.jinqigufen.top/gtcxmdqdqh.html

[U15] Py：高精度计时
来源：http://hz.jinghuilouyu.cn/gtkgmvhvku.html

t = time.perf_counter()
来源：http://hz.jinyuanbaomall.cn/gtdswllhoh.html

[U16] Py：命令行参数解析
来源：http://hz.dashuyun.cn/gtwmnzzbsj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.9152youxi.cn/gtmvgkeajb.html

[U17] Py：初始化日志
来源：http://hz.daxiang520.top/gterzruwzs.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xinyue.icu/gtuoexpzud.html

[U18] Py：预编译正则
来源：http://hz.zycfv.cn/gtxeavupwe.html

pat = re.compile(r"\d+")
来源：http://hz.mhx1999.top/gtxzsxhnwy.html

[U19] Py：正则替换带回调
来源：http://hz.shangyingyoupin.top/gtksspnrpw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.chenlongwang.top/gtuygowemo.html

[U20] Py：缓存函数结果
来源：http://hz.svipenyu.cn/gtqponkiqc.html

@functools.lru_cache(maxsize=None)
来源：http://hz.aibaodan.cn/gtgbxjxwkh.html

[U21] Py：自定义上下文管理器
来源：http://hz.shangyingyoupin.top/gtgeijsqaj.html

@contextlib.contextmanager
来源：http://hz.yj20258888.top/gtobmlmcng.html

[U22] Py：矩阵转置
来源：http://hz.zhixingplan.top/gtreitffer.html

list(zip(*m))
来源：http://hz.fengsongda.top/gtphksccrb.html

[U23] Py：分块读取大文件
来源：http://hz.xuetiantiany.cn/gtyrzqltqn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.9152youxi.cn/gtxkrnxamc.html

[U24] Py：路径操作
来源：http://hz.shanyushiyangkeji.top/gtpucsbnxq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.birdmap.top/gttpvyhazp.html

[U25] Py：CSV 按字典读
来源：http://hz.xuetiantiany.cn/gtqmnrsspa.html

csv.DictReader(f)
来源：http://hz.aibaodan.cn/gtlhdcopgb.html

[U26] Py：并发下载
来源：http://hz.gotoacloud.top/gtqdcxuufb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ivvv.top/gtnbulvfmr.html

[U27] Py：异步 HTTP
来源：http://hz.andypj.xyz/gtaezcqenl.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yj202588.top/gtbazhwmwp.html

[U28] Py：类型别名
来源：http://hz.yanxiufei.cn/gtoldegbha.html

UserId = int
来源：http://hz.ppjwa.cn/gtlummzgwc.html

[U29] Py：属性校验
来源：http://hz.sufxvd.cn/gtaedggrbw.html

@property 与 @x.setter 配合
来源：http://hz.hywenlv.cn/gtgnllgefe.html

[U30] Py：数据类
来源：http://hz.xinyue.icu/gtzgauisra.html

@dataclass(slots=True)
来源：http://hz.shzxlz.cn/gtuxvjwnpi.html

[U31] Py：单测
来源：http://hz.jqgufenzy.top/gtktgbsrco.html

python -m pytest -q
来源：http://hz.52xcode.cn/gtggmrriet.html

[U32] Py：代码格式化
来源：http://hz.smart0.xyz/gtabyiicdc.html

ruff format . && ruff check --fix .
来源：http://hz.sweek.top/gtkctpfxma.html

[U33] Py：打包发布
来源：http://hz.shanyushiyangkeji.top/gtnyezlkmv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hfpthk.cn/gtwksresfz.html

[U34] Py：判断编码
来源：http://hz.sweek.top/gtkjxaxfsb.html

chardet.detect(raw)
来源：http://hz.gogol.net.cn/gtgvnnbarp.html

[U35] Py：发送邮件
来源：http://hz.jinqigfzy.top/gtnfjhibdx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.dianchejie.cn/gthpxospwj.html

[U36] Py：定时任务
来源：http://hz.haohaochexian.top/gtprqldqtu.html

schedule.every(10).minutes.do(job)
来源：http://hz.hysaishi.cn/gtnpoyyyyt.html

[U37] Py：读写 Excel
来源：http://hz.aibaodan.cn/gttbnrdzgn.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.quarkkingdee.top/gtuahewlee.html

[U38] Py：获取脚本所在目录
来源：http://hz.sysykeji.top/gtgvnmrrud.html

Path(__file__).resolve().parent
来源：http://hz.sysykeji.top/gtqhziwohc.html

[U39] Py：判断是否在交互环境
来源：http://hz.shanyushiyangtech.top/gtlgewfrhi.html

sys.stdout.isatty()
来源：http://hz.shanyushiyangtech.top/gtuvumvaid.html

[U40] Py：打印到标准错误
来源：http://hz.xylfe.cn/gtyctsxaes.html

print("err", file=sys.stderr)
来源：http://hz.tian-w.cn/gtmkvhuirs.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xinyue.icu/gtzppcweus.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jlsjyb.cn/gtnzocqjhg.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.kuanghao11.cn/gtyxmxlzla.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yangfankeji.com/gtkqqxmdbq.html

[U43] PHP：声明命名空间
来源：http://hz.pengpengdd.cyou/gtudcirmtx.html

namespace App\Http;
来源：http://hz.chenzaomai.com/gtubdppnem.html

[U44] PHP：开启严格类型
来源：http://hz.ydjk.org.cn/gtdkvwayvi.html

declare(strict_types=1);
来源：http://hz.zhengqikj.top/gtfcvspcmu.html

[U45] PHP：类型声明与返回类型
来源：http://hz.daxiang520.top/gtfqfzldwu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gtemznmdhb.html

[U46] PHP：可空类型
来源：http://hz.c1oappe.top/gtordtxbkp.html

?string $name = null
来源：http://hz.shanyushiyangtech.top/gtjetbuwji.html

[U47] PHP：联合类型
来源：http://hz.daxiang520.top/gtdjvbqfcx.html

int|string $id
来源：http://hz.kuanghao11.cn/gtcnpyzqdr.html

[U48] PHP：纯枚举
来源：http://hz.ydjk.org.cn/gtyqgeybhe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jqgfzy.top/gttnbzrjhg.html

[U49] PHP：只读属性
来源：http://hz.ppjwa.cn/gtoautrzvv.html

public readonly string $name
来源：http://hz.vqdsnc.cn/gtatbqtbjg.html

[U50] PHP：构造器属性提升
来源：http://hz.jlsjyb.cn/gtdwfhydef.html

public function __construct(private int $id) {}
来源：http://hz.zdqjudy.top/gtiyszszjw.html

[U51] PHP：数组解构
来源：http://hz.wangdashe.top/gtcmqjwjaz.html

[$a, $b] = $arr;
来源：http://hz.tianlin.xyz/gtxwrdqbih.html

[U52] PHP：箭头函数
来源：http://hz.quarkkingdee.top/gtkeamxiqr.html

$double = fn($x) => $x * 2;
来源：http://hz.aibaodan.cn/gtormdmhzz.html

[U53] PHP：空合并运算符
来源：http://hz.haohaochexian.top/gtlvddwhzo.html

$v = $a ?? $b ?? "default";
来源：http://hz.guowangkeji.top/gtkkcgggaz.html

[U54] PHP：空安全调用
来源：http://hz.gzhubu.top/gtstcqhvhk.html

$obj?->method()
来源：http://hz.ywan-chungtsiang.top/gtcyetbcww.html

[U55] PHP：match 表达式
来源：http://hz.iojbl.cn/gtfwdobtom.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gogol.net.cn/gttckpjipg.html

[U56] PHP：命名参数
来源：http://hz.andypj.xyz/gttbxvvbse.html

f(a: 1, b: 2)
来源：http://hz.nanxuanxn.top/gtxqrawtnc.html

[U57] PHP：字符串插值
来源：http://hz.tianlin.xyz/gtammdteiu.html

"值: {$a}"
来源：http://hz.yangfankeji.com/gtvqajoxqc.html

[U58] PHP：数组三件套
来源：http://hz.jqgufenzy.top/gtxcgacpem.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sysykeji.top/gtrsgpxgey.html

[U59] PHP：自定义排序
来源：http://hz.yvedp.cn/gtnrtzfdis.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtrxecllpk.html

[U60] PHP：JSON 编解码
来源：http://hz.0kj1m.cn/gtbscvtgpp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhixingplan.top/gtturqqpem.html

[U61] PHP：正则
来源：http://hz.havefunace.top/gtkruyxdos.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenzaomai.com/gtwrbirbtz.html

[U62] PHP：日期对象
来源：http://hz.yj20258888.top/gtmvmxvrnv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yangfankeji.com/gtciiyjcgq.html


<!-- 参考信息 -->