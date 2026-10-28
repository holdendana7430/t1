代发 wailian999

[S39] C++：自定义比较器排序
来源：http://hz.birdmap.top/gtslnswjrd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jianghu66.top/gtdzmfuaok.html

[S40] C++：查找元素
来源：http://hz.jqgufenzy.top/gtjxrdatlb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jqgfzy.top/gtjkedecis.html

[S41] C++：类与构造函数
来源：http://hz.aibaodan.cn/gtvoioskob.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xuetiantiany.cn/gtcsvqoopx.html

[S42] C++：继承与虚函数
来源：http://hz.yuanzhike.top/gtssserwkj.html

class B : public Base { public: void f() override {} };
来源：http://hz.yvedp.cn/gtctsdpgfy.html

[S43] C++：智能指针
来源：http://hz.cdnleiting.top/gtqodegbdb.html

auto p = std::make_unique<int>(5);
来源：http://hz.zdqjudy.top/gtheeiunid.html

[S44] C++：引用传参
来源：http://hz.chenjidiqi.icu/gteoxhegcu.html

void inc(int &x) { ++x; }
来源：http://hz.cheryme.top/gtawutkcqa.html

[S45] C++：lambda
来源：http://hz.kuanghao11.cn/gtajhjseec.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jiagoushi.top/gtibaxcapg.html

[S46] C++：函数模板
来源：http://hz.shanyushiyangtech.top/gtounafssc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.birdmap.top/gtslrtpwhd.html

[S47] C++：结构化绑定遍历
来源：http://hz.ywan-chungtsiang.top/gttwdttejw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ehwqpu.com/gtmvpxfumk.html

[S48] C++：逐行读文件
来源：http://hz.snrcjt.cn/gtwkglgspl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sufxvd.cn/gtqaslnjcz.html

while (std::getline(in, line)) { }
来源：http://hz.ydjk.org.cn/gtrfhwasxc.html

[S49] C++：写文件
来源：http://hz.nwbrower.top/gtsojhlitx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yonumen.top/gtpaanhgjs.html

[S50] C++：格式化数字
来源：http://hz.jqgufenzy.top/gtrdyywpox.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sweek.top/gtxytqomib.html

[S51] C++：显式类型转换
来源：http://hz.gogol.net.cn/gteopxuthh.html

static_cast<double>(a) / b
来源：http://hz.ehwqpu.com/gtevcsegnu.html

[S52] C++：const 与 noexcept
来源：http://hz.sysykeji.top/gtvgxmlvjt.html

int size() const noexcept { return n_; }
来源：http://hz.jlsjyb.cn/gtucyrpajv.html

[S53] C++：移动语义
来源：http://hz.svipenyu.cn/gtedbodtgq.html

std::vector<int> w = std::move(v);
来源：http://hz.yvedp.cn/gtoqredkoj.html

[S54] C++：异常处理
来源：http://hz.hysaishi.cn/gtrcsunvzr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.meibo888.top/gtfizvwkel.html

[S55] C++：结构化绑定
来源：http://hz.zhengqikj.top/gtzhoitfbp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sxryk.cn/gtzuvffqcr.html

[S56] C++：optional
来源：http://hz.svipenyu.cn/gtvulxpnhn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jyoumei.cn/gtdyxesnzw.html

[S57] C++：编译期常量
来源：http://hz.jinqigfzy.top/gtlpgaaniz.html

constexpr int N = 10;
来源：http://hz.daria6918.cn/gtiwgxkfkq.html

[S58] C++：命名空间
来源：http://hz.jinyuanbaomall.cn/gtqactgvdu.html

namespace ns { int f() { return 1; } }
来源：http://hz.cashguo.top/gtasebzaoq.html

[S59] C++：静态断言
来源：http://hz.tianlin.xyz/gtrvaxhiir.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hammf.cn/gtvfalypwx.html

[S60] C++：遍历并删除元素
来源：http://hz.yueranfly.top/gtsooyeeqo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.wangdashe.top/gtjinvpmom.html

================================================================================
来源：http://hz.jiagoushi.top/gtbwwnllth.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.snrcjt.cn/gtljvlzbrm.html

================================================================================
来源：http://hz.316326.xyz/gtaezbydlt.html

[T01] Kotlin：Hello World
来源：http://hz.xinyue.icu/gtncnqezdv.html

println("Hello")
来源：http://hz.quarkkingdee.top/gtdcuoromo.html

[T02] Kotlin：变量
来源：http://hz.redwolf501.top/gtavcdwnrn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.vqdsnc.cn/gtmtkxlswk.html

[T03] Kotlin：字符串模板
来源：http://hz.sweek.top/gtjyeiedun.html

"值: $b"
来源：http://hz.hongshengwenyu.top/gthwwzxlnp.html

[T04] Kotlin：空安全
来源：http://hz.daxiang520.top/gtedafswio.html

val n: String? = null;  n?.length
来源：http://hz.fengsongda.top/gtxqgwmqhk.html

[T05] Kotlin：when 表达式
来源：http://hz.fengsongda.top/gtfbrltwif.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.mhx1999.top/gtrzwqinjk.html

[T06] Kotlin：集合映射
来源：http://hz.yuanzhike.top/gtwzjpieae.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.svipenyu.cn/gtizhqcvup.html

[T07] Kotlin：集合过滤
来源：http://hz.gogol.net.cn/gtdzemmbgl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pengpengdd.cyou/gtkvwnsgsn.html

[T08] Kotlin：数据类
来源：http://hz.zhoulong.xyz/gtvxzbtrxy.html

data class User(val name: String, val age: Int)
来源：http://hz.jyoumei.cn/gtkpxgychf.html

[T09] Kotlin：扩展函数
来源：http://hz.xingfuxueyuan.xyz/gtykwirgqk.html

fun String.exclaim() = this + "!"
来源：http://hz.xingfuxueyuan.xyz/gtwzgahjyh.html

[T10] Kotlin：默认参数
来源：http://hz.hammf.cn/gtfyhwjrdg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hnqzz.top/gtwcplrxmt.html

[T11] Kotlin：协程
来源：http://hz.cheryme.top/gtfbypmxxz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tianlin.xyz/gtpzmjxqmz.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtlkligftc.html

val (a, b) = Pair(1, 2)
来源：http://hz.smart0.xyz/gtwwtgpkny.html

[T13] Kotlin：只读 Map
来源：http://hz.xinyue.icu/gtqfpuzize.html

val m = mapOf("a" to 1)
来源：http://hz.vqdsnc.cn/gtsuvstjkx.html

[T14] Kotlin：循环
来源：http://hz.snrcjt.cn/gtwvwtcvur.html

for (i in 1..10) println(i)
来源：http://hz.wangshuangyany.cn/gtvmyvxjrp.html

[T15] Kotlin：接口
来源：http://hz.ehwqpu.com/gtbqztefhm.html

interface Shape { fun area(): Double }
来源：http://hz.xuanzx.com/gtcrkndbgt.html

[T16] Swift：Hello World
来源：http://hz.guowangkeji.top/gtvvigmwoj.html

print("Hello")
来源：http://hz.havefunace.top/gtybzdoiqz.html

[T17] Swift：变量与常量
来源：http://hz.pycfn.com/gtyiaehxlb.html

var a = 1;  let b = 2
来源：http://hz.ywan-chungtsiang.top/gtctmbsgbo.html

[T18] Swift：字符串插值
来源：http://hz.shangyingyoupin.top/gtcwrzzefu.html

"值: \(b)"
来源：http://hz.jianghu66.top/gtfqocavio.html

[T19] Swift：可选绑定
来源：http://hz.xuetiantiany.cn/gtreanniqe.html

if let n = opt { print(n) }
来源：http://hz.sufxvd.cn/gtfkigaqoj.html

[T20] Swift：数组操作
来源：http://hz.birdmap.top/gtjseykcou.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigfzy.top/gtkzahvnmw.html

[T21] Swift：遍历
来源：http://hz.bjfxy.top/gtkpauqgkn.html

for x in a { print(x) }
来源：http://hz.zdqjudy.top/gtzdorxjdh.html

[T22] Swift：字典
来源：http://hz.ydzc1.top/gtzsotbzqz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jqgfzy.top/gtxcdfgnju.html

[T23] Swift：函数
来源：http://hz.fengsongda.top/gtnnexjvzq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nwbrower.top/gtjkqvjiem.html

[T24] Swift：闭包
来源：http://hz.dianchejie.cn/gtqcacodtm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jlsjyb.cn/gtcvfbzcov.html

[T25] Swift：结构体
来源：http://hz.hywenlv.cn/gtvsbomfdg.html

struct P { var x: Int }
来源：http://hz.feifeiyinyue.top/gtgoyqgzub.html

[T26] Swift：类与重写
来源：http://hz.andypj.xyz/gtwgmoytnb.html

class A: Base { override func f() {} }
来源：http://hz.yanxiufei.cn/gtpqrsvqgl.html

[T27] Swift：错误处理
来源：http://hz.xinyue.icu/gtragpmtqb.html

do { try f() } catch { print(error) }
来源：http://hz.wangdashe.top/gtzywqovua.html

[T28] Swift：枚举
来源：http://hz.hfpthk.cn/gtnlzdarae.html

enum Color { case red, green }
来源：http://hz.zhiwuduotai.top/gtsjxhdpgh.html

[T29] Swift：guard 提前返回
来源：http://hz.aibaodan.cn/gtgtndxvyk.html

guard let x = opt else { return }
来源：http://hz.shangyingyoupin.top/gtjqkpmpes.html

[T30] Swift：协议
来源：http://hz.yj20258888.top/gtdilygfii.html

protocol Shape { func area() -> Double }
来源：http://hz.redwolf501.top/gtvnizsytc.html

[T31] Lua：Hello World
来源：http://hz.jinghuilouyu.cn/gtlvsauzke.html

print("Hello")
来源：http://hz.meibo888.top/gtjhypeipj.html

[T32] Lua：局部变量
来源：http://hz.yvedp.cn/gtcihdubuy.html

local a = 1
来源：http://hz.fzhhl.top/gtkadanoia.html

[T33] Lua：表（数组）
来源：http://hz.jqgufenzy.top/gtwqwvrwqb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhongyouzk.top/gtfxrlleis.html

[T34] Lua：遍历表
来源：http://hz.hysaishi.cn/gtirshcygf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hfpthk.cn/gtwpkgmebf.html

[T35] Lua：字典表
来源：http://hz.hysaishi.cn/gtnvrylurw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.andypj.xyz/gtajmawifs.html

[T36] Lua：函数
来源：http://hz.jyoumei.cn/gtzoeucnhb.html

function add(a, b) return a + b end
来源：http://hz.aibaodan.cn/gtqtbldgvz.html

[T37] Lua：字符串拼接
来源：http://hz.wangshuangyany.cn/gthezdpnwc.html

"a" .. "b"
来源：http://hz.zhengqikj.top/gthsogciem.html

[T38] Lua：条件
来源：http://hz.ydjk.org.cn/gtlfnsdhkj.html

if x > 0 then print("正") end
来源：http://hz.zdqjudy.top/gtciadygbd.html

[T39] Lua：模式匹配
来源：http://hz.9152youxi.cn/gtgpjweqog.html

string.find(s, "%d+")
来源：http://hz.zdqjudy.top/gtboviwubr.html

[T40] Lua：元表
来源：http://hz.zhiwuduotai.top/gtaacqrzsq.html

setmetatable({}, { __index = base })
来源：http://hz.zhongyouzk.top/gtahpbmehd.html

[T41] Perl：Hello World
来源：http://hz.xylfe.cn/gtqlklgnld.html

print "Hello\n";
来源：http://hz.shuidangran.top/gttnfinebs.html

[T42] Perl：变量类型
来源：http://hz.cashguo.top/gtspkbjryh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gotoacloud.top/gtvtmsfoqm.html

[T43] Perl：字符串插值
来源：http://hz.redwolf501.top/gttvvzlpwq.html

"值: $a"
来源：http://hz.guannengcc.top/gthteifhmz.html

[T44] Perl：条件
来源：http://hz.ehwqpu.com/gtmavyinfz.html

if ($a > 0) { print "正"; }
来源：http://hz.hongshengwenyu.top/gtytjhsele.html

[T45] Perl：数组遍历
来源：http://hz.hysaishi.cn/gtauyqhmcp.html

for my $x (@arr) { print $x; }
来源：http://hz.yueranfly.top/gtwcjujien.html

[T46] Perl：哈希操作
来源：http://hz.yueranfly.top/gtcsttyhuw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gzhubu.top/gtweuhfgzl.html

[T47] Perl：正则捕获
来源：http://hz.ydzc1.top/gtbiejvfzd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ydzc1.top/gtterxjbmr.html

[T48] Perl：正则替换
来源：http://hz.fzhhl.top/gtezcfnsnw.html

$s =~ s/old/new/g;
来源：http://hz.birdmap.top/gtlnlicxca.html

[T49] Perl：函数
来源：http://hz.sysykeji.top/gtvptlimpt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.iojbl.cn/gtxufqzsjy.html

[T50] Perl：逐行读文件
来源：http://hz.sweek.top/gthujidyat.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj202588.top/gtcywmqlfj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinghuilouyu.cn/gtyfjsuotk.html

[T51] Scala：Hello World
来源：http://hz.guannengcc.top/gtlfipjaix.html

println("Hello")
来源：http://hz.fengsongda.top/gtujrrmpao.html

[T52] Scala：变量
来源：http://hz.gogol.net.cn/gtymtbhlre.html

val a = 1;  var b = 2
来源：http://hz.cheryme.top/gtjgvtonmk.html

[T53] Scala：字符串插值
来源：http://hz.yonumen.top/gttihnyvyl.html

s"值: $b"
来源：http://hz.gaohongyu789.top/gttpgrlyes.html

[T54] Scala：集合映射
来源：http://hz.xziqi.cn/gtmnecsrzs.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.nanxinkj.top/gtaugxppzd.html

[T55] Scala：集合过滤
来源：http://hz.zhiwuduotai.top/gtwsuyfpau.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydjk.org.cn/gtibwdkgiz.html

[T56] Scala：样例类
来源：http://hz.jianghu66.top/gtrvypmkvo.html

case class User(name: String, age: Int)
来源：http://hz.nanxuanxn.top/gtycxpgiuz.html

[T57] Scala：模式匹配
来源：http://hz.nwbrower.top/gtwchblabb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.tanke756.top/gtbvsumwmb.html

[T58] Scala：函数定义
来源：http://hz.hysaishi.cn/gtjxlrfdvn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yonumen.top/gtsqgyjnya.html

[T59] Scala：循环
来源：http://hz.chenjidiqi.icu/gtdbkmytpi.html

for (i <- 1 to 10) println(i)
来源：http://hz.hywenlv.cn/gtwuxupymg.html

[T60] Scala：折叠
来源：http://hz.andypj.xyz/gttmldpere.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jiagoushi.top/gtmhipqeyp.html

================================================================================
来源：http://hz.guowangkeji.top/gtbtxjgena.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yonumen.top/gtdivlepbx.html

================================================================================
来源：http://hz.birdmap.top/gtjekdpfcf.html

[U01] Py：创建虚拟环境
来源：http://hz.shanyushiyangkeji.top/gtpcjpampo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hammf.cn/gtothabvdu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gaohongyu789.top/gtmowysxcf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.dashuyun.cn/gtmbqngpth.html

[U03] Py：加载 .env 配置
来源：http://hz.ybcxt.top/gtjvwiifmj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hywenlv.cn/gtqxgkhyso.html

[U04] Py：变量调试打印
来源：http://hz.yanxiufei.cn/gturxkdzsk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hammf.cn/gtjpufefkt.html

[U05] Py：列表去重且保序
来源：http://hz.fzhhl.top/gtmxjnibgk.html

list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtqdvrpaeo.html

[U06] Py：合并两个字典
来源：http://hz.dianchejie.cn/gttvzfcnyr.html

{**a, **b}
来源：http://hz.cashguo.top/gtljnjtnxt.html

[U07] Py：反转字典键值
来源：http://hz.tanke756.top/gtkuphwnqi.html

{v: k for k, v in d.items()}
来源：http://hz.zycfv.cn/gtrhqbxqmw.html

[U08] Py：展平二维列表
来源：http://hz.zhoulong.xyz/gtbclwqywk.html

[y for x in nested for y in x]
来源：http://hz.jinyuanbaomall.cn/gtcbvhtcqj.html

[U09] Py：字典取最大值的键
来源：http://hz.0kj1m.cn/gtibybrsya.html

max(d, key=d.get)
来源：http://hz.yuanzhike.top/gtkespifij.html

[U10] Py：按值排序字典
来源：http://hz.shanyushiyangkeji.top/gtwgevbzyh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.c1oappe.top/gtmkppvqee.html

[U11] Py：生成器表达式
来源：http://hz.xingfuxueyuan.xyz/gtfiiokvyh.html

(x * 2 for x in arr)
来源：http://hz.fzhhl.top/gtohapyixt.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.svipenyu.cn/gtgxxmrbxz.html

Counter(arr).most_common(3)
来源：http://hz.cucudq.cn/gtwyjurbgf.html

[U13] Py：固定长度队列
来源：http://hz.tanke756.top/gtkavpjkht.html

deque(maxlen=10)
来源：http://hz.jinghuilouyu.cn/gtzmloclbh.html

[U14] Py：分组收集到列表
来源：http://hz.kuanghao11.cn/gthmsnjtop.html

defaultdict(list)
来源：http://hz.ydzc1.top/gtqmixuppq.html

[U15] Py：高精度计时
来源：http://hz.hongshengwenyu.top/gthvheigxg.html

t = time.perf_counter()
来源：http://hz.zhijiandao.cn/gtfregpnbi.html

[U16] Py：命令行参数解析
来源：http://hz.guowangkeji.top/gtrvljvecu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xingfuxueyuan.xyz/gtrmueesdr.html

[U17] Py：初始化日志
来源：http://hz.yuxming.cn/gtgyymlmhn.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhoulong.xyz/gtjyfknehx.html

[U18] Py：预编译正则
来源：http://hz.cdnleiting.top/gtstcqqlfi.html

pat = re.compile(r"\d+")
来源：http://hz.yonumen.top/gtivgzefuo.html

[U19] Py：正则替换带回调
来源：http://hz.shuidangran.top/gtjtffoxeq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.aibaodan.cn/gtcxiqgrvt.html

[U20] Py：缓存函数结果
来源：http://hz.gogol.net.cn/gtsqpcbphc.html

@functools.lru_cache(maxsize=None)
来源：http://hz.nanxinkj.top/gtecwwlght.html

[U21] Py：自定义上下文管理器
来源：http://hz.yueranfly.top/gtuocklnxq.html

@contextlib.contextmanager
来源：http://hz.hywenlv.cn/gtvyycfkmf.html

[U22] Py：矩阵转置
来源：http://hz.jyoumei.cn/gtnbbclxle.html

list(zip(*m))
来源：http://hz.52xcode.cn/gtosbzzmft.html

[U23] Py：分块读取大文件
来源：http://hz.kuanghao11.cn/gtgcnqtefe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhengqikj.top/gtvoslihqx.html

[U24] Py：路径操作
来源：http://hz.dashuyun.cn/gtgkflvbmv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gotoacloud.top/gtfjghmukp.html

[U25] Py：CSV 按字典读
来源：http://hz.sxryk.cn/gtkxajkrgx.html

csv.DictReader(f)
来源：http://hz.sxryk.cn/gtfsojlaly.html

[U26] Py：并发下载
来源：http://hz.jiagoushi.top/gtwlhmhbyl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.daria6918.cn/gtgnygewrf.html

[U27] Py：异步 HTTP
来源：http://hz.pengpengdd.cyou/gtfkwoclgk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.gotoacloud.top/gtntutshkx.html

[U28] Py：类型别名
来源：http://hz.daria6918.cn/gtvvghauee.html

UserId = int
来源：http://hz.hywenlv.cn/gtniduhaoy.html

[U29] Py：属性校验
来源：http://hz.yuanzhike.top/gteblcctxq.html

@property 与 @x.setter 配合
来源：http://hz.tian-w.cn/gthoadpkat.html

[U30] Py：数据类
来源：http://hz.ppjwa.cn/gtdblvezpv.html

@dataclass(slots=True)
来源：http://hz.gogol.net.cn/gtiyagrcga.html

[U31] Py：单测
来源：http://hz.yuxming.cn/gtopbrltup.html

python -m pytest -q
来源：http://hz.gogol.net.cn/gteibvlkop.html

[U32] Py：代码格式化
来源：http://hz.hammf.cn/gtumzoqehn.html

ruff format . && ruff check --fix .
来源：http://hz.52xcode.cn/gtapubtwdw.html

[U33] Py：打包发布
来源：http://hz.birdmap.top/gtxiljqeja.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jlsjyb.cn/gtluzawexi.html

[U34] Py：判断编码
来源：http://hz.smart0.xyz/gtelmcmcid.html

chardet.detect(raw)
来源：http://hz.zhiwuduotai.top/gtscytqnyb.html

[U35] Py：发送邮件
来源：http://hz.ydzc1.top/gthxclgcsm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yangfankeji.com/gtllpgslts.html

[U36] Py：定时任务
来源：http://hz.chenlongwang.top/gtxblgqblx.html

schedule.every(10).minutes.do(job)
来源：http://hz.hnxiangtu.top/gtzndekhuh.html

[U37] Py：读写 Excel
来源：http://hz.ybcxt.top/gtdhclkoty.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.nanxinkj.top/gtyyketdqq.html

[U38] Py：获取脚本所在目录
来源：http://hz.havefunace.top/gthizvybjy.html

Path(__file__).resolve().parent
来源：http://hz.birdmap.top/gtirispgmy.html

[U39] Py：判断是否在交互环境
来源：http://hz.gzhubu.top/gtftnllvwu.html

sys.stdout.isatty()
来源：http://hz.yuxming.cn/gtpgetythz.html

[U40] Py：打印到标准错误
来源：http://hz.gzhubu.top/gtthgtknza.html

print("err", file=sys.stderr)
来源：http://hz.guannengcc.top/gtjihwwvvk.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ywan-chungtsiang.top/gtpzprhaep.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ppjwa.cn/gtonnszquk.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yj20258.top/gtyazmkytu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.vqdsnc.cn/gtizxfxdwv.html

[U43] PHP：声明命名空间
来源：http://hz.bjfxy.top/gtxnhwqaes.html

namespace App\Http;
来源：http://hz.snrcjt.cn/gtlshzybzc.html

[U44] PHP：开启严格类型
来源：http://hz.316326.xyz/gtolkkrrqv.html

declare(strict_types=1);
来源：http://hz.pengpengdd.cyou/gtjoblgjgb.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shzxlz.cn/gtgaevarpw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daxiang520.top/gtnpvhkzjx.html

[U46] PHP：可空类型
来源：http://hz.jinqigufen.top/gtswdztbmu.html

?string $name = null
来源：http://hz.ppjwa.cn/gttellnxmf.html

[U47] PHP：联合类型
来源：http://hz.guannengcc.top/gtzirzlshz.html

int|string $id
来源：http://hz.yuxming.cn/gtydnhukyg.html

[U48] PHP：纯枚举
来源：http://hz.hongshengwenyu.top/gtohhwecjr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xylfe.cn/gtlwunfmbr.html

[U49] PHP：只读属性
来源：http://hz.yj20258888.top/gtnvhiqitv.html

public readonly string $name
来源：http://hz.ivvv.top/gtklmenhjk.html

[U50] PHP：构造器属性提升
来源：http://hz.yueranfly.top/gtucvujnhx.html

public function __construct(private int $id) {}
来源：http://hz.xylfe.cn/gtexfahcwk.html

[U51] PHP：数组解构
来源：http://hz.xziqi.cn/gtieolaugf.html

[$a, $b] = $arr;
来源：http://hz.jinghuilouyu.cn/gttojanqmh.html

[U52] PHP：箭头函数
来源：http://hz.smart0.xyz/gttaqcdhgv.html

$double = fn($x) => $x * 2;
来源：http://hz.shzxlz.cn/gtuqvylxzb.html

[U53] PHP：空合并运算符
来源：http://hz.jinghuilouyu.cn/gtmiukzvuo.html

$v = $a ?? $b ?? "default";
来源：http://hz.quarkkingdee.top/gtxeoirptm.html

[U54] PHP：空安全调用
来源：http://hz.zhoulong.xyz/gtawhhlyxv.html

$obj?->method()
来源：http://hz.zhaomingkeji.xyz/gtbvgiisau.html

[U55] PHP：match 表达式
来源：http://hz.cqqwz.cn/gtjtsytaka.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.vqdsnc.cn/gtwatalozx.html

[U56] PHP：命名参数
来源：http://hz.zhijiandao.cn/gtzsenarcp.html

f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gtofzcvqnu.html

[U57] PHP：字符串插值
来源：http://hz.zhengqikj.top/gtaflenzbw.html

"值: {$a}"
来源：http://hz.zhengqikj.top/gtuvjdafmz.html

[U58] PHP：数组三件套
来源：http://hz.316326.xyz/gtvhwftgdh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.meibo888.top/gtcoumoflk.html

[U59] PHP：自定义排序
来源：http://hz.mhx1999.top/gtxmcjtgru.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xinyue.icu/gtyfquviko.html

[U60] PHP：JSON 编解码
来源：http://hz.dianchejie.cn/gtevravmmq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhixingplan.top/gtrofkkqci.html

[U61] PHP：正则
来源：http://hz.wangshuangyany.cn/gtiqzgekwf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hammf.cn/gtwaxselfn.html

[U62] PHP：日期对象
来源：http://hz.yueranfly.top/gtrmjmvqix.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zycfv.cn/gtsmoukmiw.html

[U63] PHP：文件读写
来源：http://hz.sysykeji.top/gtqwbwhbbk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.vqdsnc.cn/gtgswhneyg.html

[U64] PHP：目录遍历
来源：http://hz.svipenyu.cn/gtijhzuyei.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jinqigfzy.top/gtuvdxcaaj.html


<!-- 参考信息 -->