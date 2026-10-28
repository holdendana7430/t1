代发 wailian999

[S45] C++：lambda
来源：http://hz.xuetiantiany.cn/gtopilvfaq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.kuanghao11.cn/gtwkgfpija.html

[S46] C++：函数模板
来源：http://hz.quarkkingdee.top/gtfrulocup.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xinyue.icu/gtzrehhojg.html

[S47] C++：结构化绑定遍历
来源：http://hz.jlsjyb.cn/gtiwoprqzc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenzaomai.com/gtvnliiedh.html

[S48] C++：逐行读文件
来源：http://hz.yj20258.top/gttgskzlbi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tanke756.top/gtlxnyaupf.html

while (std::getline(in, line)) { }
来源：http://hz.yueranfly.top/gtmgfxetlv.html

[S49] C++：写文件
来源：http://hz.jinghuilouyu.cn/gtnoqckbnm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.0kj1m.cn/gtopdngbpj.html

[S50] C++：格式化数字
来源：http://hz.316326.xyz/gtvkranafs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.redwolf501.top/gtmnbdevjq.html

[S51] C++：显式类型转换
来源：http://hz.316326.xyz/gtnztdgbwg.html

static_cast<double>(a) / b
来源：http://hz.snrcjt.cn/gtwhvyejgl.html

[S52] C++：const 与 noexcept
来源：http://hz.jinghuilouyu.cn/gtmsowheyu.html

int size() const noexcept { return n_; }
来源：http://hz.shzxlz.cn/gtzlqwypjf.html

[S53] C++：移动语义
来源：http://hz.xinyue.icu/gtpbkxlbxf.html

std::vector<int> w = std::move(v);
来源：http://hz.iojbl.cn/gttwwqnmdx.html

[S54] C++：异常处理
来源：http://hz.yongpay.top/gtgqnpuewo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xziqi.cn/gtqimthdqx.html

[S55] C++：结构化绑定
来源：http://hz.meibo888.top/gtdpmkrtvo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.guowangkeji.top/gtsyigbrvp.html

[S56] C++：optional
来源：http://hz.hywenlv.cn/gttiyzszrc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hongshengwenyu.top/gtxaxpbrpp.html

[S57] C++：编译期常量
来源：http://hz.smart0.xyz/gtjjwtpuuw.html

constexpr int N = 10;
来源：http://hz.guannengcc.top/gtsbajboqe.html

[S58] C++：命名空间
来源：http://hz.sweek.top/gtlvvkqsru.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtbkcrqikd.html

[S59] C++：静态断言
来源：http://hz.cucudq.cn/gttieudskx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.kuanghao11.cn/gtybmcqsjw.html

[S60] C++：遍历并删除元素
来源：http://hz.dashuyun.cn/gteyxvvwhz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jqgufenzy.top/gtbkyoxjrd.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjvvkwcjl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zdqjudy.top/gttkzyxfpx.html

================================================================================
来源：http://hz.yonumen.top/gtxcbmmdhy.html

[T01] Kotlin：Hello World
来源：http://hz.aizwys.cn/gtfmwwnjmb.html

println("Hello")
来源：http://hz.shanyushiyangtech.top/gtljwudacr.html

[T02] Kotlin：变量
来源：http://hz.jqgfzy.top/gtglnjwtsk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yangfankeji.com/gttlewgxci.html

[T03] Kotlin：字符串模板
来源：http://hz.aizwys.cn/gtvxgdlvgf.html

"值: $b"
来源：http://hz.vqdsnc.cn/gtplqimsde.html

[T04] Kotlin：空安全
来源：http://hz.andypj.xyz/gtltazbuoc.html

val n: String? = null;  n?.length
来源：http://hz.gaohongyu789.top/gtvwlsijvx.html

[T05] Kotlin：when 表达式
来源：http://hz.yj202588.top/gtfheyelas.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.bjfxy.top/gtafxoukxk.html

[T06] Kotlin：集合映射
来源：http://hz.nwbrower.top/gtckonjnfq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangdashe.top/gtruiubosz.html

[T07] Kotlin：集合过滤
来源：http://hz.cheryme.top/gtterqyjfv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangtech.top/gtsvkoumuj.html

[T08] Kotlin：数据类
来源：http://hz.ywan-chungtsiang.top/gtkuyypsuh.html

data class User(val name: String, val age: Int)
来源：http://hz.daria6918.cn/gthylhlpbu.html

[T09] Kotlin：扩展函数
来源：http://hz.feifeiyinyue.top/gtutjqynxn.html

fun String.exclaim() = this + "!"
来源：http://hz.daria6918.cn/gtacyzpwjw.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigfzy.top/gtdkhequbv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.feifeiyinyue.top/gtpqqxsihp.html

[T11] Kotlin：协程
来源：http://hz.zhongyouzk.top/gtztpvqawa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hnqzz.top/gtmilsalhk.html

[T12] Kotlin：解构声明
来源：http://hz.shzxlz.cn/gthadriawk.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhaomingkeji.xyz/gtvynqejik.html

[T13] Kotlin：只读 Map
来源：http://hz.jinghuilouyu.cn/gtmdceuhox.html

val m = mapOf("a" to 1)
来源：http://hz.yueranfly.top/gtcgmzbzah.html

[T14] Kotlin：循环
来源：http://hz.hysaishi.cn/gtongtzhfy.html

for (i in 1..10) println(i)
来源：http://hz.jianghu66.top/gtfdjdzzbs.html

[T15] Kotlin：接口
来源：http://hz.tanke756.top/gtdsyjkkii.html

interface Shape { fun area(): Double }
来源：http://hz.chenlongwang.top/gtuatmjfmy.html

[T16] Swift：Hello World
来源：http://hz.svipenyu.cn/gtahuocorf.html

print("Hello")
来源：http://hz.gotoacloud.top/gtswiiulcg.html

[T17] Swift：变量与常量
来源：http://hz.316326.xyz/gtkaigxyip.html

var a = 1;  let b = 2
来源：http://hz.hongshengwenyu.top/gtkxsknlfz.html

[T18] Swift：字符串插值
来源：http://hz.sweek.top/gttzwpnrvl.html

"值: \(b)"
来源：http://hz.cqqwz.cn/gtzxpfdopk.html

[T19] Swift：可选绑定
来源：http://hz.feifeiyinyue.top/gtmcdvcxhe.html

if let n = opt { print(n) }
来源：http://hz.bjfxy.top/gtfqceliql.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtbhreprvm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.smart0.xyz/gtsdfpkjue.html

[T21] Swift：遍历
来源：http://hz.yuxming.cn/gtojjiqvim.html

for x in a { print(x) }
来源：http://hz.ybcxt.top/gtrtzwksbi.html

[T22] Swift：字典
来源：http://hz.xingfuxueyuan.xyz/gtfraszzya.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xinyue.icu/gtqeulibpw.html

[T23] Swift：函数
来源：http://hz.iojbl.cn/gtlilpxbko.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.meibo888.top/gtxjeombxz.html

[T24] Swift：闭包
来源：http://hz.xziqi.cn/gtznlnxwpj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.smart0.xyz/gtzfvbsplz.html

[T25] Swift：结构体
来源：http://hz.dashuyun.cn/gtvyqcnsui.html

struct P { var x: Int }
来源：http://hz.yanxiufei.cn/gtyergyfhr.html

[T26] Swift：类与重写
来源：http://hz.cashguo.top/gtuxfwyvqb.html

class A: Base { override func f() {} }
来源：http://hz.c1oappe.top/gthqesenfi.html

[T27] Swift：错误处理
来源：http://hz.dashuyun.cn/gtzkhkqzrm.html

do { try f() } catch { print(error) }
来源：http://hz.yangfankeji.com/gtqbhejnyn.html

[T28] Swift：枚举
来源：http://hz.zhengqikj.top/gtvqytfjkb.html

enum Color { case red, green }
来源：http://hz.ivvv.top/gtovempvug.html

[T29] Swift：guard 提前返回
来源：http://hz.yj202588.top/gtdnjrlemj.html

guard let x = opt else { return }
来源：http://hz.bjfxy.top/gtpvgeuaeq.html

[T30] Swift：协议
来源：http://hz.yonumen.top/gtncroeyhl.html

protocol Shape { func area() -> Double }
来源：http://hz.bjfxy.top/gtunbcystp.html

[T31] Lua：Hello World
来源：http://hz.ywan-chungtsiang.top/gtowrzqchb.html

print("Hello")
来源：http://hz.cqqwz.cn/gtvbliebsk.html

[T32] Lua：局部变量
来源：http://hz.tianlin.xyz/gtscgciubf.html

local a = 1
来源：http://hz.yonumen.top/gtztyfgxmc.html

[T33] Lua：表（数组）
来源：http://hz.chenjidiqi.icu/gtbbllufcc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhixingplan.top/gtimnmhcny.html

[T34] Lua：遍历表
来源：http://hz.vqdsnc.cn/gtaeoecmww.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xingfuxueyuan.xyz/gtxqpxqune.html

[T35] Lua：字典表
来源：http://hz.nwbrower.top/gtlcrjgmoe.html

local d = { a = 1 };  d.b = 2
来源：http://hz.fengsongda.top/gtduskkkgj.html

[T36] Lua：函数
来源：http://hz.guannengcc.top/gtscsxqryc.html

function add(a, b) return a + b end
来源：http://hz.redwolf501.top/gtwpeiiotm.html

[T37] Lua：字符串拼接
来源：http://hz.guowangkeji.top/gteysdsixo.html

"a" .. "b"
来源：http://hz.tian-w.cn/gtszlqacpe.html

[T38] Lua：条件
来源：http://hz.sweek.top/gttjhfhrqw.html

if x > 0 then print("正") end
来源：http://hz.vqdsnc.cn/gtugtaezso.html

[T39] Lua：模式匹配
来源：http://hz.dianchejie.cn/gttfohlspw.html

string.find(s, "%d+")
来源：http://hz.andypj.xyz/gtoynyihsj.html

[T40] Lua：元表
来源：http://hz.ehwqpu.com/gthrcvbckz.html

setmetatable({}, { __index = base })
来源：http://hz.xinyue.icu/gtnbverlqy.html

[T41] Perl：Hello World
来源：http://hz.zhixingplan.top/gtesxjubtc.html

print "Hello\n";
来源：http://hz.jinghuilouyu.cn/gtsnuwmrlq.html

[T42] Perl：变量类型
来源：http://hz.hnqzz.top/gtzhjqesle.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ehwqpu.com/gtutcxkhnc.html

[T43] Perl：字符串插值
来源：http://hz.52xcode.cn/gtarennckb.html

"值: $a"
来源：http://hz.gzhubu.top/gtauausgqb.html

[T44] Perl：条件
来源：http://hz.52xcode.cn/gtbcfjbibp.html

if ($a > 0) { print "正"; }
来源：http://hz.jqgufenzy.top/gtpridrasz.html

[T45] Perl：数组遍历
来源：http://hz.yanxiufei.cn/gtmzfyzocw.html

for my $x (@arr) { print $x; }
来源：http://hz.jqgufenzy.top/gtdzxbkaxm.html

[T46] Perl：哈希操作
来源：http://hz.yuxming.cn/gtyukwmhrz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.pengpengdd.cyou/gtwhomoqdp.html

[T47] Perl：正则捕获
来源：http://hz.guannengcc.top/gtjwjqaalx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.9152youxi.cn/gtefmukvmo.html

[T48] Perl：正则替换
来源：http://hz.fengsongda.top/gtmjgmvbsi.html

$s =~ s/old/new/g;
来源：http://hz.birdmap.top/gtytdtnkcj.html

[T49] Perl：函数
来源：http://hz.52xcode.cn/gtpstlpduk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jiagoushi.top/gtqhfrzqkz.html

[T50] Perl：逐行读文件
来源：http://hz.jlsjyb.cn/gtpczsjjxr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jlsjyb.cn/gtigeewfsu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinyuanbaomall.cn/gtpikiggmk.html

[T51] Scala：Hello World
来源：http://hz.havefunace.top/gtbuiavmzn.html

println("Hello")
来源：http://hz.jlsjyb.cn/gtxqgjuwci.html

[T52] Scala：变量
来源：http://hz.zdqjudy.top/gtyddbogfv.html

val a = 1;  var b = 2
来源：http://hz.tanke756.top/gtnodgwozq.html

[T53] Scala：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtruziwhpp.html

s"值: $b"
来源：http://hz.iojbl.cn/gtcegnydhm.html

[T54] Scala：集合映射
来源：http://hz.shanyushiyangkeji.top/gtbsoclgzy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zdqjudy.top/gtjnjainfz.html

[T55] Scala：集合过滤
来源：http://hz.jinghuilouyu.cn/gtqdkzzeob.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cdnleiting.top/gtmcqsalhh.html

[T56] Scala：样例类
来源：http://hz.cdnleiting.top/gtbbssgtup.html

case class User(name: String, age: Int)
来源：http://hz.shangyingyoupin.top/gtvpmiijdb.html

[T57] Scala：模式匹配
来源：http://hz.havefunace.top/gtbmlsgpnp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhaomingkeji.xyz/gtwqwgafep.html

[T58] Scala：函数定义
来源：http://hz.smart0.xyz/gtraszbatv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenlongwang.top/gtgaayykyb.html

[T59] Scala：循环
来源：http://hz.ppjwa.cn/gtvhazinhq.html

for (i <- 1 to 10) println(i)
来源：http://hz.meibo888.top/gtdhivkhtw.html

[T60] Scala：折叠
来源：http://hz.cucudq.cn/gtalpxyohr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.havefunace.top/gtjvqskakr.html

================================================================================
来源：http://hz.shuidangran.top/gtbzuibwok.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shuidangran.top/gthxjycrgm.html

================================================================================
来源：http://hz.yuxming.cn/gtqfxsqhml.html

[U01] Py：创建虚拟环境
来源：http://hz.jyoumei.cn/gtwfwpykfz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jyoumei.cn/gtsfdvggrw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ywan-chungtsiang.top/gtpwcyenfe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yangfankeji.com/gtiyzwqdqm.html

[U03] Py：加载 .env 配置
来源：http://hz.nwbrower.top/gtgyzexwxb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sweek.top/gtrlfhhohk.html

[U04] Py：变量调试打印
来源：http://hz.gogol.net.cn/gtiykervlj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tanke756.top/gtanvajsbt.html

[U05] Py：列表去重且保序
来源：http://hz.yonumen.top/gtqylqzjgo.html

list(dict.fromkeys(arr))
来源：http://hz.yj20258888.top/gteclszyws.html

[U06] Py：合并两个字典
来源：http://hz.zdqjudy.top/gtolireiiq.html

{**a, **b}
来源：http://hz.mhx1999.top/gtqbvattyt.html

[U07] Py：反转字典键值
来源：http://hz.dianchejie.cn/gtzfqwyjck.html

{v: k for k, v in d.items()}
来源：http://hz.aibaodan.cn/gteaxtkydj.html

[U08] Py：展平二维列表
来源：http://hz.yuxming.cn/gtsdgofuay.html

[y for x in nested for y in x]
来源：http://hz.xylfe.cn/gtewiyrswa.html

[U09] Py：字典取最大值的键
来源：http://hz.sysykeji.top/gtofufcity.html

max(d, key=d.get)
来源：http://hz.shanyushiyangkeji.top/gtsvkmfeoz.html

[U10] Py：按值排序字典
来源：http://hz.yuxming.cn/gtxhzwuqju.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cdnleiting.top/gtsxlxwwfe.html

[U11] Py：生成器表达式
来源：http://hz.hnqzz.top/gtnzswatnb.html

(x * 2 for x in arr)
来源：http://hz.sxryk.cn/gtqwburifj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhijiandao.cn/gtizgqosjl.html

Counter(arr).most_common(3)
来源：http://hz.guowangkeji.top/gtaivzgbug.html

[U13] Py：固定长度队列
来源：http://hz.ydjk.org.cn/gtfpczagez.html

deque(maxlen=10)
来源：http://hz.daxiang520.top/gtnqkiavup.html

[U14] Py：分组收集到列表
来源：http://hz.wangdashe.top/gtmqagrlxv.html

defaultdict(list)
来源：http://hz.yj20258.top/gtbetdgrhn.html

[U15] Py：高精度计时
来源：http://hz.jianghu66.top/gtiteoycwo.html

t = time.perf_counter()
来源：http://hz.yueranfly.top/gtsspjktrw.html

[U16] Py：命令行参数解析
来源：http://hz.smart0.xyz/gtzrqskmte.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sysykeji.top/gtfpsgatfn.html

[U17] Py：初始化日志
来源：http://hz.snrcjt.cn/gtuqtxoegz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yonumen.top/gtbsdrfgyu.html

[U18] Py：预编译正则
来源：http://hz.shzxlz.cn/gtmytzgwby.html

pat = re.compile(r"\d+")
来源：http://hz.chenjidiqi.icu/gtjqnrszvt.html

[U19] Py：正则替换带回调
来源：http://hz.cashguo.top/gtjfxupnga.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.gzhubu.top/gtwastcsvv.html

[U20] Py：缓存函数结果
来源：http://hz.zhengqikj.top/gtuklzlhrd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.wangdashe.top/gtvqlifdth.html

[U21] Py：自定义上下文管理器
来源：http://hz.feifeiyinyue.top/gtidpgnroa.html

@contextlib.contextmanager
来源：http://hz.jiagoushi.top/gtkvabeslf.html

[U22] Py：矩阵转置
来源：http://hz.zhongyouzk.top/gtxfxxsthf.html

list(zip(*m))
来源：http://hz.smart0.xyz/gtuuhuiskr.html

[U23] Py：分块读取大文件
来源：http://hz.cdnleiting.top/gtelgpxbll.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cheryme.top/gtlvvuabos.html

[U24] Py：路径操作
来源：http://hz.cqqwz.cn/gtbslmnklx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ehwqpu.com/gtiwqkaaak.html

[U25] Py：CSV 按字典读
来源：http://hz.hongshengwenyu.top/gtowjxhzmb.html

csv.DictReader(f)
来源：http://hz.pengpengdd.cyou/gtdbisdwfc.html

[U26] Py：并发下载
来源：http://hz.0kj1m.cn/gtokgwfeia.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.chenzaomai.com/gtgyvclnqb.html

[U27] Py：异步 HTTP
来源：http://hz.sxryk.cn/gtwyodncbm.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.fzhhl.top/gtenxyuxze.html

[U28] Py：类型别名
来源：http://hz.xingfuxueyuan.xyz/gtaoeduzsq.html

UserId = int
来源：http://hz.cheryme.top/gtwgmywjtz.html

[U29] Py：属性校验
来源：http://hz.andypj.xyz/gtsvostslx.html

@property 与 @x.setter 配合
来源：http://hz.ehwqpu.com/gtjhwplzvn.html

[U30] Py：数据类
来源：http://hz.andypj.xyz/gtcsfeerar.html

@dataclass(slots=True)
来源：http://hz.guowangkeji.top/gtwpwoukem.html

[U31] Py：单测
来源：http://hz.ywan-chungtsiang.top/gtbojxfqkz.html

python -m pytest -q
来源：http://hz.quarkkingdee.top/gturojgexo.html

[U32] Py：代码格式化
来源：http://hz.jinqigfzy.top/gttfwkeduj.html

ruff format . && ruff check --fix .
来源：http://hz.gogol.net.cn/gtgjdbjwll.html

[U33] Py：打包发布
来源：http://hz.yuanzhike.top/gtyzyhtbxh.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.andypj.xyz/gtonpvfcmj.html

[U34] Py：判断编码
来源：http://hz.ivvv.top/gtrkbvsohz.html

chardet.detect(raw)
来源：http://hz.c1oappe.top/gtbtguqqmg.html

[U35] Py：发送邮件
来源：http://hz.jinyuanbaomall.cn/gtgguludst.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.wangdashe.top/gtscibefzx.html

[U36] Py：定时任务
来源：http://hz.sysykeji.top/gtgmmgudqj.html

schedule.every(10).minutes.do(job)
来源：http://hz.nwbrower.top/gtkdegonpn.html

[U37] Py：读写 Excel
来源：http://hz.gotoacloud.top/gtqbsjthpq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.cashguo.top/gtlovwtwtd.html

[U38] Py：获取脚本所在目录
来源：http://hz.nanxinkj.top/gthbplkzhr.html

Path(__file__).resolve().parent
来源：http://hz.andypj.xyz/gtczhmfxrb.html

[U39] Py：判断是否在交互环境
来源：http://hz.ivvv.top/gtxlsrappb.html

sys.stdout.isatty()
来源：http://hz.jyoumei.cn/gtavszvebj.html

[U40] Py：打印到标准错误
来源：http://hz.ivvv.top/gtxbvxmjhm.html

print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtavfwojon.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenlongwang.top/gtvuajdzxn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.haohaochexian.top/gtdcjtbpow.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.wangshuangyany.cn/gtrkiwbsxm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.guannengcc.top/gtgdjbnrss.html

[U43] PHP：声明命名空间
来源：http://hz.jqgufenzy.top/gtfrjqjivw.html

namespace App\Http;
来源：http://hz.tianlin.xyz/gtjvqaxvvb.html

[U44] PHP：开启严格类型
来源：http://hz.fengsongda.top/gttnrsabye.html

declare(strict_types=1);
来源：http://hz.xinyue.icu/gtgssptcji.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cdnleiting.top/gtynypevxr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtzjcjymae.html

[U46] PHP：可空类型
来源：http://hz.zhaomingkeji.xyz/gthiuimjcz.html

?string $name = null
来源：http://hz.chenjidiqi.icu/gtjwalixza.html

[U47] PHP：联合类型
来源：http://hz.c1oappe.top/gtyoqxpfpv.html

int|string $id
来源：http://hz.snrcjt.cn/gtrpdwodbs.html

[U48] PHP：纯枚举
来源：http://hz.iojbl.cn/gtvcjdmrpv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinghuilouyu.cn/gtrodbekcw.html

[U49] PHP：只读属性
来源：http://hz.meibo888.top/gtqsvyoosl.html

public readonly string $name
来源：http://hz.hammf.cn/gtfuborhdp.html

[U50] PHP：构造器属性提升
来源：http://hz.yuxming.cn/gtfewnkxtn.html

public function __construct(private int $id) {}
来源：http://hz.gzhubu.top/gtvbfuunfc.html

[U51] PHP：数组解构
来源：http://hz.zhijiandao.cn/gtldygjcii.html

[$a, $b] = $arr;
来源：http://hz.yj202588.top/gtxtwpbdaa.html

[U52] PHP：箭头函数
来源：http://hz.wangshuangyany.cn/gtvuetmnnj.html

$double = fn($x) => $x * 2;
来源：http://hz.yuanzhike.top/gtayakiufk.html

[U53] PHP：空合并运算符
来源：http://hz.jinqigufen.top/gtutznxdps.html

$v = $a ?? $b ?? "default";
来源：http://hz.jiagoushi.top/gtxgwlslmh.html

[U54] PHP：空安全调用
来源：http://hz.nanxinkj.top/gtimbdaset.html

$obj?->method()
来源：http://hz.316326.xyz/gtgevibavu.html

[U55] PHP：match 表达式
来源：http://hz.hongshengwenyu.top/gtpicdeiwj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hywenlv.cn/gtsgscavgv.html

[U56] PHP：命名参数
来源：http://hz.ehwqpu.com/gtrchkpjfe.html

f(a: 1, b: 2)
来源：http://hz.yangfankeji.com/gtgrfnuirn.html

[U57] PHP：字符串插值
来源：http://hz.fengsongda.top/gtttugjsew.html

"值: {$a}"
来源：http://hz.gogol.net.cn/gtdgqjoyty.html

[U58] PHP：数组三件套
来源：http://hz.aibaodan.cn/gtqwntzutp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yj20258888.top/gtruwswtxt.html

[U59] PHP：自定义排序
来源：http://hz.guowangkeji.top/gtimxsaymd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.kuanghao11.cn/gtelbujzvy.html

[U60] PHP：JSON 编解码
来源：http://hz.sxryk.cn/gtdboxgeqp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj20258888.top/gtvyukivro.html

[U61] PHP：正则
来源：http://hz.jinqigfzy.top/gtacsgbisl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.gotoacloud.top/gtffjagnkp.html

[U62] PHP：日期对象
来源：http://hz.hnxiangtu.top/gttiedcmwq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.meibo888.top/gtntyqjurc.html

[U63] PHP：文件读写
来源：http://hz.wangshuangyany.cn/gtwzaquboi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.snrcjt.cn/gtbsksvdyj.html

[U64] PHP：目录遍历
来源：http://hz.gaohongyu789.top/gtdlajneyt.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.shanyushiyangkeji.top/gtkwobzxip.html

[U65] PHP：会话
来源：http://hz.tanke756.top/gtwzygtikn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.c1oappe.top/gtonnwgdpc.html

[U66] PHP：设置 Cookie
来源：http://hz.yongpay.top/gtcpyfidix.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gogol.net.cn/gtbbonqbpq.html

[U67] PHP：处理文件上传
来源：http://hz.0kj1m.cn/gtpeftfdqt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.tanke756.top/gttpplbbzz.html

[U68] PHP：PDO 连接
来源：http://hz.smart0.xyz/gttoyegghz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jiagoushi.top/gtypqjchln.html

[U69] PHP：PDO 预处理
来源：http://hz.zhengqikj.top/gtbblpjjcg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.dashuyun.cn/gterfcadzo.html

[U70] PHP：PDO 事务
来源：http://hz.jqgufenzy.top/gtaitthcya.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jinyuanbaomall.cn/gtspnzkqrw.html


<!-- 参考信息 -->