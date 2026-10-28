代发 wailian999

[S43] C++：智能指针
来源：http://hz.9152youxi.cn/gtvjbokade.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuxming.cn/gteblydesy.html

[S44] C++：引用传参
来源：http://hz.sxryk.cn/gtikomfeio.html

void inc(int &x) { ++x; }
来源：http://hz.316326.xyz/gtpqluyhhn.html

[S45] C++：lambda
来源：http://hz.shuidangran.top/gtgwbjgabj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guowangkeji.top/gtpchrqyyn.html

[S46] C++：函数模板
来源：http://hz.bjfxy.top/gtqnjpjejd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.andypj.xyz/gtvrzkdaqa.html

[S47] C++：结构化绑定遍历
来源：http://hz.aizwys.cn/gtgkwiplfk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yanxiufei.cn/gtioawiqpi.html

[S48] C++：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtmgyoyplk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.smart0.xyz/gtacuvuqpp.html

while (std::getline(in, line)) { }
来源：http://hz.hongshengwenyu.top/gtkmfdyjea.html

[S49] C++：写文件
来源：http://hz.yongpay.top/gtxthbwupo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shanyushiyangkeji.top/gthllwwucw.html

[S50] C++：格式化数字
来源：http://hz.hnxiangtu.top/gtcvktyvdb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.birdmap.top/gtxbdbbvod.html

[S51] C++：显式类型转换
来源：http://hz.hammf.cn/gtmkswfvit.html

static_cast<double>(a) / b
来源：http://hz.jianghu66.top/gtdkcezpcn.html

[S52] C++：const 与 noexcept
来源：http://hz.0kj1m.cn/gtxxrmtcqv.html

int size() const noexcept { return n_; }
来源：http://hz.shangyingyoupin.top/gtxowsfter.html

[S53] C++：移动语义
来源：http://hz.ivvv.top/gtmysojlvx.html

std::vector<int> w = std::move(v);
来源：http://hz.yongpay.top/gtnwofqbax.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gtxcrkgzwu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guowangkeji.top/gtohotbyea.html

[S55] C++：结构化绑定
来源：http://hz.9152youxi.cn/gtxsusfslp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.snrcjt.cn/gtefhqlpnc.html

[S56] C++：optional
来源：http://hz.zhijiandao.cn/gtsngkhzwi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yuanzhike.top/gttrrbyqwf.html

[S57] C++：编译期常量
来源：http://hz.zhongyouzk.top/gtaqivfowi.html

constexpr int N = 10;
来源：http://hz.yuxming.cn/gtijtfbilj.html

[S58] C++：命名空间
来源：http://hz.iojbl.cn/gtaunltqat.html

namespace ns { int f() { return 1; } }
来源：http://hz.sysykeji.top/gttwrijpsw.html

[S59] C++：静态断言
来源：http://hz.fengsongda.top/gtmevyghyw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sysykeji.top/gtfwuflzdu.html

[S60] C++：遍历并删除元素
来源：http://hz.yueranfly.top/gtrboujhec.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yongpay.top/gtbzyagjgo.html

================================================================================
来源：http://hz.yj20258.top/gtitretxdk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydjk.org.cn/gttbwbvhuw.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcuguwomi.html

[T01] Kotlin：Hello World
来源：http://hz.jqgufenzy.top/gtzymyttah.html

println("Hello")
来源：http://hz.shzxlz.cn/gtfvyguioh.html

[T02] Kotlin：变量
来源：http://hz.zdqjudy.top/gtgnlxnilw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yongpay.top/gtkmqrynlf.html

[T03] Kotlin：字符串模板
来源：http://hz.gaohongyu789.top/gtnpfkdecv.html

"值: $b"
来源：http://hz.pycfn.com/gtizrfcdxh.html

[T04] Kotlin：空安全
来源：http://hz.shangyingyoupin.top/gtadaowylq.html

val n: String? = null;  n?.length
来源：http://hz.nanxuanxn.top/gtfpwsyglm.html

[T05] Kotlin：when 表达式
来源：http://hz.xuanzx.com/gtmacwjjth.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenzaomai.com/gtmngbsbtc.html

[T06] Kotlin：集合映射
来源：http://hz.fengsongda.top/gthqqqydzs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xylfe.cn/gtpibcumoa.html

[T07] Kotlin：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtbyudraop.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hywenlv.cn/gtmvrooxoe.html

[T08] Kotlin：数据类
来源：http://hz.cdnleiting.top/gtqfopbxiq.html

data class User(val name: String, val age: Int)
来源：http://hz.gotoacloud.top/gtkwuvpcjc.html

[T09] Kotlin：扩展函数
来源：http://hz.quarkkingdee.top/gtgtydjcop.html

fun String.exclaim() = this + "!"
来源：http://hz.52xcode.cn/gtozskemgc.html

[T10] Kotlin：默认参数
来源：http://hz.yueranfly.top/gtymnzhays.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gaohongyu789.top/gtuuaxljqw.html

[T11] Kotlin：协程
来源：http://hz.haohaochexian.top/gtmhfdhxxg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yj20258.top/gtbpjyhgeu.html

[T12] Kotlin：解构声明
来源：http://hz.hammf.cn/gtoafjrzqq.html

val (a, b) = Pair(1, 2)
来源：http://hz.sweek.top/gtejzuglvd.html

[T13] Kotlin：只读 Map
来源：http://hz.xingfuxueyuan.xyz/gtbkjhnjum.html

val m = mapOf("a" to 1)
来源：http://hz.zhijiandao.cn/gthedzaflo.html

[T14] Kotlin：循环
来源：http://hz.yuxming.cn/gtiztwcozc.html

for (i in 1..10) println(i)
来源：http://hz.c1oappe.top/gtduhxcxtl.html

[T15] Kotlin：接口
来源：http://hz.svipenyu.cn/gtjlkvbmsm.html

interface Shape { fun area(): Double }
来源：http://hz.dashuyun.cn/gtyaoleogt.html

[T16] Swift：Hello World
来源：http://hz.yj20258.top/gteyerjubh.html

print("Hello")
来源：http://hz.dianchejie.cn/gtdviyoyic.html

[T17] Swift：变量与常量
来源：http://hz.sufxvd.cn/gtllodpoov.html

var a = 1;  let b = 2
来源：http://hz.guowangkeji.top/gtjmkzllnl.html

[T18] Swift：字符串插值
来源：http://hz.shuidangran.top/gtgphtekhe.html

"值: \(b)"
来源：http://hz.dashuyun.cn/gtejlpkmlo.html

[T19] Swift：可选绑定
来源：http://hz.mhx1999.top/gtwdwzuiwk.html

if let n = opt { print(n) }
来源：http://hz.iojbl.cn/gtetokshuc.html

[T20] Swift：数组操作
来源：http://hz.tianlin.xyz/gthtrzhizp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.guannengcc.top/gtoibztwkd.html

[T21] Swift：遍历
来源：http://hz.ivvv.top/gtaaiyslul.html

for x in a { print(x) }
来源：http://hz.hysaishi.cn/gtzevrrvgz.html

[T22] Swift：字典
来源：http://hz.yj20258888.top/gtivvknjlx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gzhubu.top/gtmdalwzzo.html

[T23] Swift：函数
来源：http://hz.yj202588.top/gtcotduetv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yj202588.top/gthijniogo.html

[T24] Swift：闭包
来源：http://hz.ydjk.org.cn/gtsbixvawt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenzaomai.com/gtsnwejwdo.html

[T25] Swift：结构体
来源：http://hz.tianlin.xyz/gtrpxeuoeh.html

struct P { var x: Int }
来源：http://hz.ybcxt.top/gtfahsrkgw.html

[T26] Swift：类与重写
来源：http://hz.jqgfzy.top/gthvepowkt.html

class A: Base { override func f() {} }
来源：http://hz.nwbrower.top/gtqywccweh.html

[T27] Swift：错误处理
来源：http://hz.sysykeji.top/gtihgupwza.html

do { try f() } catch { print(error) }
来源：http://hz.dianchejie.cn/gtbsedviyh.html

[T28] Swift：枚举
来源：http://hz.xingfuxueyuan.xyz/gtsikeuvdc.html

enum Color { case red, green }
来源：http://hz.hfpthk.cn/gtkdxilufe.html

[T29] Swift：guard 提前返回
来源：http://hz.zhoulong.xyz/gtkphonzrk.html

guard let x = opt else { return }
来源：http://hz.yongpay.top/gtbxfqmewo.html

[T30] Swift：协议
来源：http://hz.daria6918.cn/gtcqudcnkg.html

protocol Shape { func area() -> Double }
来源：http://hz.zhijiandao.cn/gteruzbalj.html

[T31] Lua：Hello World
来源：http://hz.zdqjudy.top/gtxmfqjugu.html

print("Hello")
来源：http://hz.ydzc1.top/gtcyksxpni.html

[T32] Lua：局部变量
来源：http://hz.zhijiandao.cn/gtbvtphjvk.html

local a = 1
来源：http://hz.jqgfzy.top/gtevnnnyka.html

[T33] Lua：表（数组）
来源：http://hz.tian-w.cn/gtlwiluqtk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.fzhhl.top/gtnrbxzcts.html

[T34] Lua：遍历表
来源：http://hz.xuanzx.com/gtejwflekz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.bjfxy.top/gtegdeksnb.html

[T35] Lua：字典表
来源：http://hz.xylfe.cn/gtrelnkysa.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yuxming.cn/gtqffclxms.html

[T36] Lua：函数
来源：http://hz.aibaodan.cn/gtkiysshrz.html

function add(a, b) return a + b end
来源：http://hz.svipenyu.cn/gtvczwhvyo.html

[T37] Lua：字符串拼接
来源：http://hz.jiagoushi.top/gtobetdptf.html

"a" .. "b"
来源：http://hz.snrcjt.cn/gtnxtqqrwn.html

[T38] Lua：条件
来源：http://hz.yj20258888.top/gtpkzoirqk.html

if x > 0 then print("正") end
来源：http://hz.nanxinkj.top/gtkuzrqdvx.html

[T39] Lua：模式匹配
来源：http://hz.chenzaomai.com/gtmnwupyvv.html

string.find(s, "%d+")
来源：http://hz.gzhubu.top/gtrocpxsqb.html

[T40] Lua：元表
来源：http://hz.52xcode.cn/gtdrleguyi.html

setmetatable({}, { __index = base })
来源：http://hz.shzxlz.cn/gtgdnvaynb.html

[T41] Perl：Hello World
来源：http://hz.quarkkingdee.top/gtjudutzdz.html

print "Hello\n";
来源：http://hz.jianghu66.top/gtuhonxuki.html

[T42] Perl：变量类型
来源：http://hz.xuanzx.com/gtfafwtomd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.svipenyu.cn/gtsgbljkiz.html

[T43] Perl：字符串插值
来源：http://hz.quarkkingdee.top/gtyzuufbfo.html

"值: $a"
来源：http://hz.pycfn.com/gtsddjmiie.html

[T44] Perl：条件
来源：http://hz.gaohongyu789.top/gtwkcygyjv.html

if ($a > 0) { print "正"; }
来源：http://hz.0kj1m.cn/gtpieugsqr.html

[T45] Perl：数组遍历
来源：http://hz.ybcxt.top/gtltrcofsq.html

for my $x (@arr) { print $x; }
来源：http://hz.andypj.xyz/gtuwvxqwgk.html

[T46] Perl：哈希操作
来源：http://hz.snrcjt.cn/gtfqaeingx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cheryme.top/gtdhflxgch.html

[T47] Perl：正则捕获
来源：http://hz.gzhubu.top/gtaxvxnfkn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangtech.top/gtgkllnxqq.html

[T48] Perl：正则替换
来源：http://hz.hysaishi.cn/gtlnjgosbl.html

$s =~ s/old/new/g;
来源：http://hz.tian-w.cn/gtualvfhsz.html

[T49] Perl：函数
来源：http://hz.cucudq.cn/gtyqetjcsl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jqgfzy.top/gtmmkkhmyq.html

[T50] Perl：逐行读文件
来源：http://hz.cheryme.top/gtmzgdsapj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigufen.top/gtyvfffrxd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yuxming.cn/gtzhviymll.html

[T51] Scala：Hello World
来源：http://hz.yj20258888.top/gtgirbdxak.html

println("Hello")
来源：http://hz.yueranfly.top/gtoxafgysh.html

[T52] Scala：变量
来源：http://hz.cdnleiting.top/gtejvexzgz.html

val a = 1;  var b = 2
来源：http://hz.hongshengwenyu.top/gtrdsiwvxo.html

[T53] Scala：字符串插值
来源：http://hz.wangshuangyany.cn/gtcveephwo.html

s"值: $b"
来源：http://hz.gogol.net.cn/gtdzqpegkk.html

[T54] Scala：集合映射
来源：http://hz.yuanzhike.top/gtqeqefnlm.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zycfv.cn/gtnhkvlujw.html

[T55] Scala：集合过滤
来源：http://hz.cashguo.top/gthrqjkfty.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sweek.top/gtuzbcowwu.html

[T56] Scala：样例类
来源：http://hz.smart0.xyz/gtnrogajnh.html

case class User(name: String, age: Int)
来源：http://hz.feifeiyinyue.top/gtrloeexqu.html

[T57] Scala：模式匹配
来源：http://hz.tanke756.top/gthmucfork.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.aibaodan.cn/gthinahtll.html

[T58] Scala：函数定义
来源：http://hz.snrcjt.cn/gtslbqdooy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cashguo.top/gthrzgjjbl.html

[T59] Scala：循环
来源：http://hz.redwolf501.top/gtaajenkza.html

for (i <- 1 to 10) println(i)
来源：http://hz.cashguo.top/gtnflefatr.html

[T60] Scala：折叠
来源：http://hz.daria6918.cn/gtlhxqgolt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shanyushiyangkeji.top/gtxbqlmkml.html

================================================================================
来源：http://hz.xinyue.icu/gtwapcwghm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.dianchejie.cn/gtpbekavqp.html

================================================================================
来源：http://hz.yonumen.top/gtqrjsehwl.html

[U01] Py：创建虚拟环境
来源：http://hz.gogol.net.cn/gtgyonuqbt.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tian-w.cn/gtefmijyfd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shanyushiyangkeji.top/gtarhuorcs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ppjwa.cn/gtkbvmprsj.html

[U03] Py：加载 .env 配置
来源：http://hz.yvedp.cn/gtfgmrxnyq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.cdnleiting.top/gthpcuecez.html

[U04] Py：变量调试打印
来源：http://hz.snrcjt.cn/gttxqmktvc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.wangdashe.top/gtrnaipaqp.html

[U05] Py：列表去重且保序
来源：http://hz.dashuyun.cn/gtkipuasan.html

list(dict.fromkeys(arr))
来源：http://hz.daria6918.cn/gtceidwhwe.html

[U06] Py：合并两个字典
来源：http://hz.yj20258.top/gtvvsvmjue.html

{**a, **b}
来源：http://hz.dashuyun.cn/gtoyaybsfa.html

[U07] Py：反转字典键值
来源：http://hz.tanke756.top/gtvmoesaio.html

{v: k for k, v in d.items()}
来源：http://hz.guannengcc.top/gttscdszot.html

[U08] Py：展平二维列表
来源：http://hz.xuetiantiany.cn/gtnrgzzmtk.html

[y for x in nested for y in x]
来源：http://hz.tanke756.top/gtnzymbgpi.html

[U09] Py：字典取最大值的键
来源：http://hz.jyoumei.cn/gtybsmnpji.html

max(d, key=d.get)
来源：http://hz.xylfe.cn/gtrhlxoqoq.html

[U10] Py：按值排序字典
来源：http://hz.andypj.xyz/gthycwguqc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhoulong.xyz/gtehxsifwv.html

[U11] Py：生成器表达式
来源：http://hz.ydjk.org.cn/gtjavxumgp.html

(x * 2 for x in arr)
来源：http://hz.yongpay.top/gtydbsoumn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.kuanghao11.cn/gtkwrclyak.html

Counter(arr).most_common(3)
来源：http://hz.shanyushiyangtech.top/gtfqxxmsog.html

[U13] Py：固定长度队列
来源：http://hz.nwbrower.top/gtgrmdazld.html

deque(maxlen=10)
来源：http://hz.gaohongyu789.top/gtcymgcqmd.html

[U14] Py：分组收集到列表
来源：http://hz.yueranfly.top/gtbvnwvale.html

defaultdict(list)
来源：http://hz.yueranfly.top/gtawsyibzb.html

[U15] Py：高精度计时
来源：http://hz.jianghu66.top/gtqcriuixt.html

t = time.perf_counter()
来源：http://hz.cdnleiting.top/gtanpoiqtc.html

[U16] Py：命令行参数解析
来源：http://hz.tian-w.cn/gtdgorqoyi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhixingplan.top/gtofmojbiv.html

[U17] Py：初始化日志
来源：http://hz.cheryme.top/gtbfjaehwi.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xziqi.cn/gtdqmpqodz.html

[U18] Py：预编译正则
来源：http://hz.hnxiangtu.top/gtfhbrdczi.html

pat = re.compile(r"\d+")
来源：http://hz.fzhhl.top/gtcaayknrc.html

[U19] Py：正则替换带回调
来源：http://hz.sufxvd.cn/gtpopezdmz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ywan-chungtsiang.top/gthxxbpkqu.html

[U20] Py：缓存函数结果
来源：http://hz.kuanghao11.cn/gtkioexgzn.html

@functools.lru_cache(maxsize=None)
来源：http://hz.tianlin.xyz/gtagqpgedj.html

[U21] Py：自定义上下文管理器
来源：http://hz.jiagoushi.top/gtiondqsvk.html

@contextlib.contextmanager
来源：http://hz.9152youxi.cn/gtjssqdsts.html

[U22] Py：矩阵转置
来源：http://hz.yueranfly.top/gtsbbzajxk.html

list(zip(*m))
来源：http://hz.nwbrower.top/gtupgesbab.html

[U23] Py：分块读取大文件
来源：http://hz.zhixingplan.top/gtjclhrinf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hongshengwenyu.top/gtyhvwlqsp.html

[U24] Py：路径操作
来源：http://hz.jinghuilouyu.cn/gtaedacjdf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.mhx1999.top/gtecklvoxq.html

[U25] Py：CSV 按字典读
来源：http://hz.gotoacloud.top/gtwtcjxobb.html

csv.DictReader(f)
来源：http://hz.smart0.xyz/gtwbodoniq.html

[U26] Py：并发下载
来源：http://hz.sysykeji.top/gtclnlfbba.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.havefunace.top/gtyppnmxks.html

[U27] Py：异步 HTTP
来源：http://hz.iojbl.cn/gtknunwtxf.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.chenjidiqi.icu/gttetwxqsq.html

[U28] Py：类型别名
来源：http://hz.yuxming.cn/gtbdycknhd.html

UserId = int
来源：http://hz.mhx1999.top/gtljkksfdp.html

[U29] Py：属性校验
来源：http://hz.guowangkeji.top/gtbsmildhr.html

@property 与 @x.setter 配合
来源：http://hz.gaohongyu789.top/gtnkahlymh.html

[U30] Py：数据类
来源：http://hz.cheryme.top/gtgsxhexrq.html

@dataclass(slots=True)
来源：http://hz.yuxming.cn/gtmxcpfstr.html

[U31] Py：单测
来源：http://hz.c1oappe.top/gtlsvfyxlu.html

python -m pytest -q
来源：http://hz.gotoacloud.top/gtzbmcouuf.html

[U32] Py：代码格式化
来源：http://hz.jiagoushi.top/gtpnpyqfrc.html

ruff format . && ruff check --fix .
来源：http://hz.sweek.top/gtyxcvcfxz.html

[U33] Py：打包发布
来源：http://hz.cucudq.cn/gtyhxypxxm.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jqgfzy.top/gtchzcwucx.html

[U34] Py：判断编码
来源：http://hz.9152youxi.cn/gtvukkwrjr.html

chardet.detect(raw)
来源：http://hz.nwbrower.top/gtmmohmbqq.html

[U35] Py：发送邮件
来源：http://hz.xylfe.cn/gtybwcmohw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jianghu66.top/gthxxbdukr.html

[U36] Py：定时任务
来源：http://hz.zhiwuduotai.top/gtgmxshtya.html

schedule.every(10).minutes.do(job)
来源：http://hz.jinqigfzy.top/gtaavngefq.html

[U37] Py：读写 Excel
来源：http://hz.fengsongda.top/gtutxytrhv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.gogol.net.cn/gtcemruaym.html

[U38] Py：获取脚本所在目录
来源：http://hz.smart0.xyz/gtkurfcarw.html

Path(__file__).resolve().parent
来源：http://hz.wangshuangyany.cn/gtwbpvsovr.html

[U39] Py：判断是否在交互环境
来源：http://hz.dashuyun.cn/gtwddsxnbb.html

sys.stdout.isatty()
来源：http://hz.tanke756.top/gtvkpeeeec.html

[U40] Py：打印到标准错误
来源：http://hz.zhengqikj.top/gtfdnomroh.html

print("err", file=sys.stderr)
来源：http://hz.kuanghao11.cn/gtaeubmtqx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jqgfzy.top/gtptlvmfku.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jiagoushi.top/gtyofxpehq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jlsjyb.cn/gtmykjdmyn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yj20258.top/gthhlfasbm.html

[U43] PHP：声明命名空间
来源：http://hz.hfpthk.cn/gtodlnbkbk.html

namespace App\Http;
来源：http://hz.smart0.xyz/gtvluvowkt.html

[U44] PHP：开启严格类型
来源：http://hz.gogol.net.cn/gtbeohylbp.html

declare(strict_types=1);
来源：http://hz.aibaodan.cn/gtjkwirhfs.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhongyouzk.top/gtmfjvkfpy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtpdoprrsc.html

[U46] PHP：可空类型
来源：http://hz.sufxvd.cn/gtaizfzunj.html

?string $name = null
来源：http://hz.hywenlv.cn/gtxjkgehzz.html

[U47] PHP：联合类型
来源：http://hz.xziqi.cn/gtlffdpmvk.html

int|string $id
来源：http://hz.hysaishi.cn/gtoqretdkl.html

[U48] PHP：纯枚举
来源：http://hz.nwbrower.top/gtenhwsvwn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yonumen.top/gtqtjxmion.html

[U49] PHP：只读属性
来源：http://hz.daxiang520.top/gteenpnzoc.html

public readonly string $name
来源：http://hz.ybcxt.top/gtadhgbvgh.html

[U50] PHP：构造器属性提升
来源：http://hz.guannengcc.top/gtwpvmstup.html

public function __construct(private int $id) {}
来源：http://hz.feifeiyinyue.top/gthotvoljs.html

[U51] PHP：数组解构
来源：http://hz.ivvv.top/gtycjnnkqb.html

[$a, $b] = $arr;
来源：http://hz.xinyue.icu/gtdxlzryma.html

[U52] PHP：箭头函数
来源：http://hz.zdqjudy.top/gtgcgluzex.html

$double = fn($x) => $x * 2;
来源：http://hz.bjfxy.top/gtlinnthhh.html

[U53] PHP：空合并运算符
来源：http://hz.hnxiangtu.top/gthjdykpqs.html

$v = $a ?? $b ?? "default";
来源：http://hz.cashguo.top/gtvhbkvedd.html

[U54] PHP：空安全调用
来源：http://hz.ywan-chungtsiang.top/gtcrhojvqy.html

$obj?->method()
来源：http://hz.xziqi.cn/gtzzwtmosg.html

[U55] PHP：match 表达式
来源：http://hz.guannengcc.top/gtoaqrhaqy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zdqjudy.top/gtgzxaxssj.html

[U56] PHP：命名参数
来源：http://hz.hnxiangtu.top/gtxhdazbtf.html

f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtiwyhozkf.html

[U57] PHP：字符串插值
来源：http://hz.316326.xyz/gtezulfelg.html

"值: {$a}"
来源：http://hz.jianghu66.top/gtsvxqeggz.html

[U58] PHP：数组三件套
来源：http://hz.jinqigfzy.top/gtilyqlpig.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jiagoushi.top/gttmvtvjur.html

[U59] PHP：自定义排序
来源：http://hz.aizwys.cn/gtyqyikynx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258888.top/gtshskdviu.html

[U60] PHP：JSON 编解码
来源：http://hz.aizwys.cn/gtetawsvof.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cheryme.top/gtziruitqi.html

[U61] PHP：正则
来源：http://hz.316326.xyz/gtirzfydve.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cheryme.top/gtbmuekbox.html

[U62] PHP：日期对象
来源：http://hz.daria6918.cn/gtcostggzi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ywan-chungtsiang.top/gtijfzeldz.html

[U63] PHP：文件读写
来源：http://hz.quarkkingdee.top/gtbjkvuxtq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhijiandao.cn/gtmrbqnuzj.html

[U64] PHP：目录遍历
来源：http://hz.fzhhl.top/gtnfmejyfn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.wangdashe.top/gtvlzfinra.html

[U65] PHP：会话
来源：http://hz.hammf.cn/gtpphauthm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.nwbrower.top/gthhqfjyoy.html

[U66] PHP：设置 Cookie
来源：http://hz.ydjk.org.cn/gtrxxwsgxq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhijiandao.cn/gtnwiglyyz.html

[U67] PHP：处理文件上传
来源：http://hz.9152youxi.cn/gtydrfjpzn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xuanzx.com/gtolnffacz.html

[U68] PHP：PDO 连接
来源：http://hz.ydjk.org.cn/gtepczzkmm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cqqwz.cn/gtprybhyye.html


<!-- 参考信息 -->