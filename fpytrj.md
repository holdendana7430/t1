代发 wailian999

[S37] C++：set
来源：http://hz.0kj1m.cn/gtezbuzlrt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hfpthk.cn/gtqylmfhzb.html

[S38] C++：排序
来源：http://hz.jyoumei.cn/gtfvjhvczk.html

std::sort(v.begin(), v.end());
来源：http://hz.ydzc1.top/gtuxbeosas.html

[S39] C++：自定义比较器排序
来源：http://hz.c1oappe.top/gtmresnopd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jiagoushi.top/gtdpejwnxo.html

[S40] C++：查找元素
来源：http://hz.hnxiangtu.top/gtzedefiqk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.316326.xyz/gthqovxrvz.html

[S41] C++：类与构造函数
来源：http://hz.guowangkeji.top/gtizgxqgkw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ppjwa.cn/gtfoehbule.html

[S42] C++：继承与虚函数
来源：http://hz.jyoumei.cn/gtyzhfbbic.html

class B : public Base { public: void f() override {} };
来源：http://hz.aizwys.cn/gtwgfkoddq.html

[S43] C++：智能指针
来源：http://hz.shanyushiyangkeji.top/gtzzxtzggr.html

auto p = std::make_unique<int>(5);
来源：http://hz.zycfv.cn/gtopycjhnw.html

[S44] C++：引用传参
来源：http://hz.zdqjudy.top/gtjkhfcgty.html

void inc(int &x) { ++x; }
来源：http://hz.meibo888.top/gtyiihsxkx.html

[S45] C++：lambda
来源：http://hz.chenjidiqi.icu/gtrbqpufxh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jqgfzy.top/gtwrxzembo.html

[S46] C++：函数模板
来源：http://hz.wangshuangyany.cn/gtzczejsht.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangtech.top/gtdhvwezcz.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhengqikj.top/gtsvziroap.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.fengsongda.top/gttjbdkruj.html

[S48] C++：逐行读文件
来源：http://hz.xuetiantiany.cn/gteciwbkqo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtrncnvmsc.html

while (std::getline(in, line)) { }
来源：http://hz.zhoulong.xyz/gtfcmhaene.html

[S49] C++：写文件
来源：http://hz.bjfxy.top/gtirrcbtam.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenzaomai.com/gtunkmjnmk.html

[S50] C++：格式化数字
来源：http://hz.0kj1m.cn/gtrtpaovrm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.iojbl.cn/gtbzojnwhr.html

[S51] C++：显式类型转换
来源：http://hz.yuanzhike.top/gtkvvcoyvs.html

static_cast<double>(a) / b
来源：http://hz.mhx1999.top/gtoldxmirq.html

[S52] C++：const 与 noexcept
来源：http://hz.jinqigufen.top/gtwjyofjok.html

int size() const noexcept { return n_; }
来源：http://hz.bjfxy.top/gtlgwermei.html

[S53] C++：移动语义
来源：http://hz.quarkkingdee.top/gtymfxkoqv.html

std::vector<int> w = std::move(v);
来源：http://hz.hnxiangtu.top/gtxstmtaar.html

[S54] C++：异常处理
来源：http://hz.jinyuanbaomall.cn/gtmlmtjhaz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zycfv.cn/gtbhqvmdgx.html

[S55] C++：结构化绑定
来源：http://hz.daxiang520.top/gtdjxqmzbz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sxryk.cn/gtcoiewckw.html

[S56] C++：optional
来源：http://hz.ydzc1.top/gtujjedmip.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guowangkeji.top/gtornrrugm.html

[S57] C++：编译期常量
来源：http://hz.nanxinkj.top/gtjnfrgvrr.html

constexpr int N = 10;
来源：http://hz.gogol.net.cn/gtzmipuidl.html

[S58] C++：命名空间
来源：http://hz.gaohongyu789.top/gtqnhaifxy.html

namespace ns { int f() { return 1; } }
来源：http://hz.aizwys.cn/gtjuhoqzto.html

[S59] C++：静态断言
来源：http://hz.chenjidiqi.icu/gtkgoetona.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yvedp.cn/gtsjffbcdc.html

[S60] C++：遍历并删除元素
来源：http://hz.yongpay.top/gtifkuwahm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xingfuxueyuan.xyz/gtjhzmmcfy.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtyieyrqdm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ppjwa.cn/gtyldvggfp.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtlfmmacvl.html

[T01] Kotlin：Hello World
来源：http://hz.smart0.xyz/gtrzchmuyd.html

println("Hello")
来源：http://hz.aizwys.cn/gtsetisppz.html

[T02] Kotlin：变量
来源：http://hz.hfpthk.cn/gtnoaspfbv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhengqikj.top/gtbfhvcdmo.html

[T03] Kotlin：字符串模板
来源：http://hz.yj202588.top/gtzifvjboj.html

"值: $b"
来源：http://hz.cqqwz.cn/gtbivyoqtl.html

[T04] Kotlin：空安全
来源：http://hz.zhengqikj.top/gtgfhxjrik.html

val n: String? = null;  n?.length
来源：http://hz.snrcjt.cn/gthauanyre.html

[T05] Kotlin：when 表达式
来源：http://hz.sysykeji.top/gtqkvehfda.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hywenlv.cn/gtintpeoiz.html

[T06] Kotlin：集合映射
来源：http://hz.aibaodan.cn/gttxfqoefu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yongpay.top/gtgdborzva.html

[T07] Kotlin：集合过滤
来源：http://hz.hysaishi.cn/gtbukajoye.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yongpay.top/gtinuvpqhw.html

[T08] Kotlin：数据类
来源：http://hz.sufxvd.cn/gtsohlxnpy.html

data class User(val name: String, val age: Int)
来源：http://hz.zhijiandao.cn/gtqixtxxeh.html

[T09] Kotlin：扩展函数
来源：http://hz.zdqjudy.top/gtlfpfksgr.html

fun String.exclaim() = this + "!"
来源：http://hz.fzhhl.top/gtckxuoocp.html

[T10] Kotlin：默认参数
来源：http://hz.xinyue.icu/gtvwtwacrp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hammf.cn/gtwfiksdpu.html

[T11] Kotlin：协程
来源：http://hz.0kj1m.cn/gtxtkqhcml.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ywan-chungtsiang.top/gtujcrvksi.html

[T12] Kotlin：解构声明
来源：http://hz.yj202588.top/gtkgxygvrr.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhongyouzk.top/gtzrlqkuly.html

[T13] Kotlin：只读 Map
来源：http://hz.shzxlz.cn/gtonspjezm.html

val m = mapOf("a" to 1)
来源：http://hz.gotoacloud.top/gtopzwgjbw.html

[T14] Kotlin：循环
来源：http://hz.nwbrower.top/gtiegvgrfo.html

for (i in 1..10) println(i)
来源：http://hz.52xcode.cn/gtopqzwpfq.html

[T15] Kotlin：接口
来源：http://hz.aizwys.cn/gtkaxdskms.html

interface Shape { fun area(): Double }
来源：http://hz.0kj1m.cn/gtxhypwlps.html

[T16] Swift：Hello World
来源：http://hz.zhoulong.xyz/gtpzeynqmj.html

print("Hello")
来源：http://hz.iojbl.cn/gtiwwvutdx.html

[T17] Swift：变量与常量
来源：http://hz.zhiwuduotai.top/gtambvrdzp.html

var a = 1;  let b = 2
来源：http://hz.yj202588.top/gtchijyfab.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtkpevajme.html

"值: \(b)"
来源：http://hz.ppjwa.cn/gtghdzzbbk.html

[T19] Swift：可选绑定
来源：http://hz.redwolf501.top/gtsmcqoarb.html

if let n = opt { print(n) }
来源：http://hz.hnxiangtu.top/gtvnailoia.html

[T20] Swift：数组操作
来源：http://hz.316326.xyz/gtvovzlzwb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhaomingkeji.xyz/gtaobrrexg.html

[T21] Swift：遍历
来源：http://hz.52xcode.cn/gtwtdazsxl.html

for x in a { print(x) }
来源：http://hz.ywan-chungtsiang.top/gtgeklnuog.html

[T22] Swift：字典
来源：http://hz.sufxvd.cn/gtfvgcefbk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sysykeji.top/gtrkzcpvnb.html

[T23] Swift：函数
来源：http://hz.jyoumei.cn/gtktfvyxwr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.dianchejie.cn/gtboxqirnk.html

[T24] Swift：闭包
来源：http://hz.xylfe.cn/gtelddqtqr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hnxiangtu.top/gtnniuxacw.html

[T25] Swift：结构体
来源：http://hz.ivvv.top/gtplfzbywd.html

struct P { var x: Int }
来源：http://hz.zhongyouzk.top/gtaegpoedr.html

[T26] Swift：类与重写
来源：http://hz.shuidangran.top/gtuahwidgt.html

class A: Base { override func f() {} }
来源：http://hz.xziqi.cn/gtqmmpwucd.html

[T27] Swift：错误处理
来源：http://hz.smart0.xyz/gtotqkfgyb.html

do { try f() } catch { print(error) }
来源：http://hz.feifeiyinyue.top/gttdvzmbsc.html

[T28] Swift：枚举
来源：http://hz.xuetiantiany.cn/gtfaaykprj.html

enum Color { case red, green }
来源：http://hz.cheryme.top/gtfkkzmwck.html

[T29] Swift：guard 提前返回
来源：http://hz.yuxming.cn/gtlxsliszy.html

guard let x = opt else { return }
来源：http://hz.52xcode.cn/gtnccdascs.html

[T30] Swift：协议
来源：http://hz.daria6918.cn/gtczjllgkk.html

protocol Shape { func area() -> Double }
来源：http://hz.yvedp.cn/gtxrkkzsqd.html

[T31] Lua：Hello World
来源：http://hz.xinyue.icu/gtfwfczpxi.html

print("Hello")
来源：http://hz.ydzc1.top/gtuhisuwlf.html

[T32] Lua：局部变量
来源：http://hz.zhoulong.xyz/gtsziwbwne.html

local a = 1
来源：http://hz.cqqwz.cn/gtoljfmljz.html

[T33] Lua：表（数组）
来源：http://hz.yonumen.top/gtglwbxkub.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cucudq.cn/gtvgmncwpi.html

[T34] Lua：遍历表
来源：http://hz.cashguo.top/gtmcdfrayg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cashguo.top/gtcxcilwwc.html

[T35] Lua：字典表
来源：http://hz.iojbl.cn/gteptyvoeu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hywenlv.cn/gtkavhyxau.html

[T36] Lua：函数
来源：http://hz.yuxming.cn/gtvoyqcceu.html

function add(a, b) return a + b end
来源：http://hz.jqgufenzy.top/gtnhjfpgbc.html

[T37] Lua：字符串拼接
来源：http://hz.sxryk.cn/gtojqvfhlh.html

"a" .. "b"
来源：http://hz.zhijiandao.cn/gtpignchmn.html

[T38] Lua：条件
来源：http://hz.52xcode.cn/gtqkswafhx.html

if x > 0 then print("正") end
来源：http://hz.ydjk.org.cn/gtiebxdjww.html

[T39] Lua：模式匹配
来源：http://hz.mhx1999.top/gtrrrwzgra.html

string.find(s, "%d+")
来源：http://hz.ybcxt.top/gtmtwtnbfr.html

[T40] Lua：元表
来源：http://hz.fengsongda.top/gtqtyimfzu.html

setmetatable({}, { __index = base })
来源：http://hz.shanyushiyangtech.top/gtvldgjolv.html

[T41] Perl：Hello World
来源：http://hz.smart0.xyz/gttwxfdmzu.html

print "Hello\n";
来源：http://hz.gogol.net.cn/gtefuccalc.html

[T42] Perl：变量类型
来源：http://hz.tanke756.top/gtojfutwoj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.andypj.xyz/gtcbewnsnl.html

[T43] Perl：字符串插值
来源：http://hz.havefunace.top/gttaqyaqam.html

"值: $a"
来源：http://hz.yonumen.top/gtzlzujhtd.html

[T44] Perl：条件
来源：http://hz.ydzc1.top/gtefprphae.html

if ($a > 0) { print "正"; }
来源：http://hz.quarkkingdee.top/gtygqriujy.html

[T45] Perl：数组遍历
来源：http://hz.jyoumei.cn/gtynikegje.html

for my $x (@arr) { print $x; }
来源：http://hz.daxiang520.top/gtvrilviqm.html

[T46] Perl：哈希操作
来源：http://hz.cqqwz.cn/gtiqjykcpc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xuetiantiany.cn/gtjghjayfj.html

[T47] Perl：正则捕获
来源：http://hz.cqqwz.cn/gtbjtgzshk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhijiandao.cn/gtpzqautrx.html

[T48] Perl：正则替换
来源：http://hz.cheryme.top/gtmbwomrdo.html

$s =~ s/old/new/g;
来源：http://hz.andypj.xyz/gtrgrshpor.html

[T49] Perl：函数
来源：http://hz.jqgfzy.top/gtwukvsssm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hammf.cn/gtoqgphsud.html

[T50] Perl：逐行读文件
来源：http://hz.guowangkeji.top/gtblfpttcy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ydjk.org.cn/gtppelrrkh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.haohaochexian.top/gtewjyvaoz.html

[T51] Scala：Hello World
来源：http://hz.yonumen.top/gtscwstuzo.html

println("Hello")
来源：http://hz.shzxlz.cn/gtyqdgsxwk.html

[T52] Scala：变量
来源：http://hz.pengpengdd.cyou/gtztuexail.html

val a = 1;  var b = 2
来源：http://hz.mhx1999.top/gtvsiznxcg.html

[T53] Scala：字符串插值
来源：http://hz.yj202588.top/gtqsoxqxqe.html

s"值: $b"
来源：http://hz.ybcxt.top/gtlpnsteuh.html

[T54] Scala：集合映射
来源：http://hz.cashguo.top/gtwaflvkns.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.birdmap.top/gteofnapsc.html

[T55] Scala：集合过滤
来源：http://hz.wangdashe.top/gtexsqargw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.nanxuanxn.top/gtyyqmxdmd.html

[T56] Scala：样例类
来源：http://hz.guowangkeji.top/gtpqegqyuv.html

case class User(name: String, age: Int)
来源：http://hz.52xcode.cn/gtoprnadli.html

[T57] Scala：模式匹配
来源：http://hz.guowangkeji.top/gtegqxgzlt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.mhx1999.top/gtogrrewxh.html

[T58] Scala：函数定义
来源：http://hz.xziqi.cn/gtbpgmgspq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shzxlz.cn/gtkawdaeix.html

[T59] Scala：循环
来源：http://hz.guowangkeji.top/gtuefxvxvx.html

for (i <- 1 to 10) println(i)
来源：http://hz.nwbrower.top/gtioozttlp.html

[T60] Scala：折叠
来源：http://hz.yueranfly.top/gteoyqauey.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.9152youxi.cn/gtkhkwtqyq.html

================================================================================
来源：http://hz.ivvv.top/gtxgqeltkd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.9152youxi.cn/gtjwpihmht.html

================================================================================
来源：http://hz.yangfankeji.com/gtvbzswhxa.html

[U01] Py：创建虚拟环境
来源：http://hz.meibo888.top/gtkolnysrx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.c1oappe.top/gtjvsbkibv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jiagoushi.top/gtgsabdpea.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sxryk.cn/gtskqtkwbd.html

[U03] Py：加载 .env 配置
来源：http://hz.cdnleiting.top/gtebwukhre.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yuanzhike.top/gtuivkfyso.html

[U04] Py：变量调试打印
来源：http://hz.andypj.xyz/gtjnxyilhg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.quarkkingdee.top/gtsplnpmro.html

[U05] Py：列表去重且保序
来源：http://hz.dashuyun.cn/gtddsyveey.html

list(dict.fromkeys(arr))
来源：http://hz.jiagoushi.top/gtuwlymqjk.html

[U06] Py：合并两个字典
来源：http://hz.hywenlv.cn/gtatlolfyy.html

{**a, **b}
来源：http://hz.xingfuxueyuan.xyz/gtuutnajyb.html

[U07] Py：反转字典键值
来源：http://hz.andypj.xyz/gtbaqcvdby.html

{v: k for k, v in d.items()}
来源：http://hz.zhaomingkeji.xyz/gtpndjyosj.html

[U08] Py：展平二维列表
来源：http://hz.jinghuilouyu.cn/gtaawdmwsx.html

[y for x in nested for y in x]
来源：http://hz.jinqigfzy.top/gthjiihrqg.html

[U09] Py：字典取最大值的键
来源：http://hz.quarkkingdee.top/gtjwaparhu.html

max(d, key=d.get)
来源：http://hz.ppjwa.cn/gtizrpibvi.html

[U10] Py：按值排序字典
来源：http://hz.xinyue.icu/gtgvwfvrxn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cheryme.top/gttzzvdliy.html

[U11] Py：生成器表达式
来源：http://hz.chenlongwang.top/gtbtzeegtg.html

(x * 2 for x in arr)
来源：http://hz.quarkkingdee.top/gtvhwyngyv.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhaomingkeji.xyz/gtdjxmlucx.html

Counter(arr).most_common(3)
来源：http://hz.dashuyun.cn/gtgdigqdwl.html

[U13] Py：固定长度队列
来源：http://hz.andypj.xyz/gtyztzcesb.html

deque(maxlen=10)
来源：http://hz.yuanzhike.top/gtlqbfmejm.html

[U14] Py：分组收集到列表
来源：http://hz.hnqzz.top/gtohkowoxb.html

defaultdict(list)
来源：http://hz.zhoulong.xyz/gtufraijnr.html

[U15] Py：高精度计时
来源：http://hz.zhaomingkeji.xyz/gtaycbhkre.html

t = time.perf_counter()
来源：http://hz.yuanzhike.top/gtaoqxcrmy.html

[U16] Py：命令行参数解析
来源：http://hz.iojbl.cn/gtdmzhoxkv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xuetiantiany.cn/gtrahpuazd.html

[U17] Py：初始化日志
来源：http://hz.fengsongda.top/gthdapwziz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yongpay.top/gtpduokdxb.html

[U18] Py：预编译正则
来源：http://hz.xuanzx.com/gtrejwelyr.html

pat = re.compile(r"\d+")
来源：http://hz.yueranfly.top/gtqkvimoka.html

[U19] Py：正则替换带回调
来源：http://hz.aizwys.cn/gtqzsnrsln.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sysykeji.top/gtzvflivff.html

[U20] Py：缓存函数结果
来源：http://hz.shanyushiyangkeji.top/gtkddtwlax.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhaomingkeji.xyz/gtytjsxnzr.html

[U21] Py：自定义上下文管理器
来源：http://hz.hnqzz.top/gtsbrsmdvb.html

@contextlib.contextmanager
来源：http://hz.yanxiufei.cn/gtvnzswthg.html

[U22] Py：矩阵转置
来源：http://hz.chenjidiqi.icu/gtnvdqnmhf.html

list(zip(*m))
来源：http://hz.hnqzz.top/gtyzlbjrst.html

[U23] Py：分块读取大文件
来源：http://hz.yanxiufei.cn/gthcjgvkji.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jinyuanbaomall.cn/gtxoftpozr.html

[U24] Py：路径操作
来源：http://hz.yj20258.top/gtmixbrsew.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.daria6918.cn/gtzptfnjhw.html

[U25] Py：CSV 按字典读
来源：http://hz.yj20258888.top/gtnjfbqcni.html

csv.DictReader(f)
来源：http://hz.ydjk.org.cn/gttcfwzvnv.html

[U26] Py：并发下载
来源：http://hz.gotoacloud.top/gtvmcsabpr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.chenzaomai.com/gtharacefz.html

[U27] Py：异步 HTTP
来源：http://hz.ydzc1.top/gtkvagmhhz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.tian-w.cn/gtbgclztlb.html

[U28] Py：类型别名
来源：http://hz.9152youxi.cn/gtwerxszlj.html

UserId = int
来源：http://hz.zhixingplan.top/gtzsqlexsa.html

[U29] Py：属性校验
来源：http://hz.mhx1999.top/gtvlcvxecm.html

@property 与 @x.setter 配合
来源：http://hz.52xcode.cn/gtmrmheefx.html

[U30] Py：数据类
来源：http://hz.sysykeji.top/gtlegykahz.html

@dataclass(slots=True)
来源：http://hz.cheryme.top/gtbrmhexux.html

[U31] Py：单测
来源：http://hz.redwolf501.top/gtmgqdtedq.html

python -m pytest -q
来源：http://hz.hnqzz.top/gtaxkzxvww.html

[U32] Py：代码格式化
来源：http://hz.chenlongwang.top/gtljwocdzj.html

ruff format . && ruff check --fix .
来源：http://hz.haohaochexian.top/gtebcaofqj.html

[U33] Py：打包发布
来源：http://hz.havefunace.top/gtjrdjicln.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shuidangran.top/gtspzaybcg.html

[U34] Py：判断编码
来源：http://hz.ydjk.org.cn/gtyztsdcra.html

chardet.detect(raw)
来源：http://hz.zhaomingkeji.xyz/gtsgyqejjl.html

[U35] Py：发送邮件
来源：http://hz.gaohongyu789.top/gtbobgizen.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.wangshuangyany.cn/gtjpinqjkm.html

[U36] Py：定时任务
来源：http://hz.nanxuanxn.top/gtzyrnmric.html

schedule.every(10).minutes.do(job)
来源：http://hz.jianghu66.top/gtiibkpfee.html

[U37] Py：读写 Excel
来源：http://hz.yonumen.top/gtfrzzxtuu.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hongshengwenyu.top/gtkhffpngm.html

[U38] Py：获取脚本所在目录
来源：http://hz.tian-w.cn/gtsavwrdjv.html

Path(__file__).resolve().parent
来源：http://hz.svipenyu.cn/gteklbrapn.html

[U39] Py：判断是否在交互环境
来源：http://hz.jyoumei.cn/gtrqeuipxa.html

sys.stdout.isatty()
来源：http://hz.xziqi.cn/gtbwwoiugf.html

[U40] Py：打印到标准错误
来源：http://hz.yj202588.top/gtdnzopapj.html

print("err", file=sys.stderr)
来源：http://hz.cdnleiting.top/gtqbzqhofx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.316326.xyz/gtlpatimth.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shanyushiyangtech.top/gtpiadtsuz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hywenlv.cn/gtffphctok.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gzhubu.top/gtcyzzpjou.html

[U43] PHP：声明命名空间
来源：http://hz.daxiang520.top/gtiwsqdsve.html

namespace App\Http;
来源：http://hz.jyoumei.cn/gtdjvrkgtx.html

[U44] PHP：开启严格类型
来源：http://hz.ppjwa.cn/gtzgibfqhj.html

declare(strict_types=1);
来源：http://hz.ydzc1.top/gtftrvnusp.html

[U45] PHP：类型声明与返回类型
来源：http://hz.dashuyun.cn/gtbpmhdltf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.havefunace.top/gtpbppgohl.html

[U46] PHP：可空类型
来源：http://hz.hammf.cn/gtaogxbroq.html

?string $name = null
来源：http://hz.jinqigufen.top/gtsdtigwyc.html

[U47] PHP：联合类型
来源：http://hz.gaohongyu789.top/gtzjblmrld.html

int|string $id
来源：http://hz.c1oappe.top/gtoilvjhhk.html

[U48] PHP：纯枚举
来源：http://hz.sxryk.cn/gtoziajxfi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.iojbl.cn/gtriboobio.html

[U49] PHP：只读属性
来源：http://hz.tanke756.top/gteqsfvexj.html

public readonly string $name
来源：http://hz.iojbl.cn/gtgfrqbdby.html

[U50] PHP：构造器属性提升
来源：http://hz.hnqzz.top/gtvrdcjhpn.html

public function __construct(private int $id) {}
来源：http://hz.shzxlz.cn/gtfefnhygj.html

[U51] PHP：数组解构
来源：http://hz.ivvv.top/gtrunjjpbs.html

[$a, $b] = $arr;
来源：http://hz.haohaochexian.top/gtvbvcyolj.html

[U52] PHP：箭头函数
来源：http://hz.c1oappe.top/gtmplawxio.html

$double = fn($x) => $x * 2;
来源：http://hz.sweek.top/gtvawflbxz.html

[U53] PHP：空合并运算符
来源：http://hz.dashuyun.cn/gtnhglpizi.html

$v = $a ?? $b ?? "default";
来源：http://hz.chenjidiqi.icu/gtncrmghsc.html

[U54] PHP：空安全调用
来源：http://hz.jlsjyb.cn/gtwbrndeat.html

$obj?->method()
来源：http://hz.guowangkeji.top/gtnblfudlq.html

[U55] PHP：match 表达式
来源：http://hz.zhaomingkeji.xyz/gtcdpnjgpt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shzxlz.cn/gtwgyljbkw.html

[U56] PHP：命名参数
来源：http://hz.shzxlz.cn/gtpryfknej.html

f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtyxllnkog.html

[U57] PHP：字符串插值
来源：http://hz.hnxiangtu.top/gtmaoxlrme.html

"值: {$a}"
来源：http://hz.zhongyouzk.top/gtlqcnurtl.html

[U58] PHP：数组三件套
来源：http://hz.jiagoushi.top/gtegsiodcn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.bjfxy.top/gtdxutjgzo.html

[U59] PHP：自定义排序
来源：http://hz.smart0.xyz/gtwrhymtfc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenlongwang.top/gtnjsipnlm.html

[U60] PHP：JSON 编解码
来源：http://hz.andypj.xyz/gtehddnmzi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.sysykeji.top/gtybsnchea.html

[U61] PHP：正则
来源：http://hz.c1oappe.top/gtoahrykuo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jianghu66.top/gtkuruznfx.html

[U62] PHP：日期对象
来源：http://hz.dianchejie.cn/gtbhdpfblx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.fzhhl.top/gteamvfnka.html


<!-- 参考信息 -->