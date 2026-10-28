代发 wailian999

[S45] C++：lambda
来源：http://hz.hysaishi.cn/gtzbzkqoxq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jlsjyb.cn/gtzqmsqpxe.html

[S46] C++：函数模板
来源：http://hz.hongshengwenyu.top/gtkfkinovs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.haohaochexian.top/gtsiblhfka.html

[S47] C++：结构化绑定遍历
来源：http://hz.zycfv.cn/gthgzvukhb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.52xcode.cn/gtghnlmkwb.html

[S48] C++：逐行读文件
来源：http://hz.tianlin.xyz/gtanurigqz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.quarkkingdee.top/gthnwilajy.html

while (std::getline(in, line)) { }
来源：http://hz.jiagoushi.top/gtycbjxdvs.html

[S49] C++：写文件
来源：http://hz.sweek.top/gttwrnjzae.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gogol.net.cn/gtdxsfnxzx.html

[S50] C++：格式化数字
来源：http://hz.bjfxy.top/gtryfevymy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gaohongyu789.top/gtjlpnrafw.html

[S51] C++：显式类型转换
来源：http://hz.zycfv.cn/gtikermnde.html

static_cast<double>(a) / b
来源：http://hz.yvedp.cn/gtipaadjsf.html

[S52] C++：const 与 noexcept
来源：http://hz.zhongyouzk.top/gtqzqqaqfc.html

int size() const noexcept { return n_; }
来源：http://hz.sysykeji.top/gtcgzxxymv.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gtlgwjdkpm.html

std::vector<int> w = std::move(v);
来源：http://hz.nanxuanxn.top/gtviaglknc.html

[S54] C++：异常处理
来源：http://hz.yj20258888.top/gtlbgdkuwi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.pengpengdd.cyou/gtghuiuejs.html

[S55] C++：结构化绑定
来源：http://hz.jianghu66.top/gtrcdvcigk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zycfv.cn/gtggpdgzrv.html

[S56] C++：optional
来源：http://hz.guowangkeji.top/gtbjpwpzzr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zycfv.cn/gtvilnvlhp.html

[S57] C++：编译期常量
来源：http://hz.yonumen.top/gtysruuxrk.html

constexpr int N = 10;
来源：http://hz.yuxming.cn/gtlcphrrmp.html

[S58] C++：命名空间
来源：http://hz.xuetiantiany.cn/gtbwnrbetc.html

namespace ns { int f() { return 1; } }
来源：http://hz.vqdsnc.cn/gtketimvwj.html

[S59] C++：静态断言
来源：http://hz.havefunace.top/gtsgjdhkfw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.52xcode.cn/gtqjfoqrom.html

[S60] C++：遍历并删除元素
来源：http://hz.0kj1m.cn/gtijkcfykw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.snrcjt.cn/gtqwcjfzlz.html

================================================================================
来源：http://hz.haohaochexian.top/gtucvonngf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.birdmap.top/gtmmpcjpiu.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtnqiwduwn.html

[T01] Kotlin：Hello World
来源：http://hz.jqgfzy.top/gttvuxhqnp.html

println("Hello")
来源：http://hz.yuxming.cn/gtpwgubejy.html

[T02] Kotlin：变量
来源：http://hz.snrcjt.cn/gtgdsyrzvm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhixingplan.top/gtglovgmid.html

[T03] Kotlin：字符串模板
来源：http://hz.sysykeji.top/gtusznxucw.html

"值: $b"
来源：http://hz.nanxinkj.top/gtktdsrolw.html

[T04] Kotlin：空安全
来源：http://hz.kuanghao11.cn/gtjekzmosa.html

val n: String? = null;  n?.length
来源：http://hz.zhongyouzk.top/gtuckbceyf.html

[T05] Kotlin：when 表达式
来源：http://hz.bjfxy.top/gtudncsosl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.kuanghao11.cn/gtkkqefqfc.html

[T06] Kotlin：集合映射
来源：http://hz.zhengqikj.top/gtvrcyhdmb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cheryme.top/gtqcxuqnfq.html

[T07] Kotlin：集合过滤
来源：http://hz.hammf.cn/gtnneihufd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yvedp.cn/gthtmfgxlj.html

[T08] Kotlin：数据类
来源：http://hz.ppjwa.cn/gtqqxugzbp.html

data class User(val name: String, val age: Int)
来源：http://hz.hongshengwenyu.top/gtuiekojhh.html

[T09] Kotlin：扩展函数
来源：http://hz.shuidangran.top/gtlnchrdbr.html

fun String.exclaim() = this + "!"
来源：http://hz.jlsjyb.cn/gtyrtbshbz.html

[T10] Kotlin：默认参数
来源：http://hz.nwbrower.top/gtpdzdcfwu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.mhx1999.top/gtusxwyccx.html

[T11] Kotlin：协程
来源：http://hz.xingfuxueyuan.xyz/gtegqwnhuc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yj20258888.top/gtkyalrhal.html

[T12] Kotlin：解构声明
来源：http://hz.kuanghao11.cn/gtoblsmsvj.html

val (a, b) = Pair(1, 2)
来源：http://hz.shuidangran.top/gtnjytcfnl.html

[T13] Kotlin：只读 Map
来源：http://hz.meibo888.top/gtxuytenwa.html

val m = mapOf("a" to 1)
来源：http://hz.gaohongyu789.top/gtzjdrbxuh.html

[T14] Kotlin：循环
来源：http://hz.yongpay.top/gtbhjstfjv.html

for (i in 1..10) println(i)
来源：http://hz.chenjidiqi.icu/gtmfbisnac.html

[T15] Kotlin：接口
来源：http://hz.jinghuilouyu.cn/gtzigxbrpx.html

interface Shape { fun area(): Double }
来源：http://hz.ppjwa.cn/gtiftvfqkd.html

[T16] Swift：Hello World
来源：http://hz.sweek.top/gtijtxgxtb.html

print("Hello")
来源：http://hz.meibo888.top/gtnyjbrhbh.html

[T17] Swift：变量与常量
来源：http://hz.jinqigufen.top/gtmfhhbajz.html

var a = 1;  let b = 2
来源：http://hz.daxiang520.top/gtkbyxzdda.html

[T18] Swift：字符串插值
来源：http://hz.yangfankeji.com/gtgqtrruws.html

"值: \(b)"
来源：http://hz.316326.xyz/gtvjsttpgb.html

[T19] Swift：可选绑定
来源：http://hz.jyoumei.cn/gtoymvaeuz.html

if let n = opt { print(n) }
来源：http://hz.ppjwa.cn/gtypdiezmq.html

[T20] Swift：数组操作
来源：http://hz.cucudq.cn/gtufggfwab.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jyoumei.cn/gtgadvcret.html

[T21] Swift：遍历
来源：http://hz.jinqigufen.top/gtqjpvcuny.html

for x in a { print(x) }
来源：http://hz.hammf.cn/gtwgzrxbvu.html

[T22] Swift：字典
来源：http://hz.hongshengwenyu.top/gtdkrljgyi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnxiangtu.top/gtjzkzybuf.html

[T23] Swift：函数
来源：http://hz.iojbl.cn/gteobvwyly.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhongyouzk.top/gtqqhzprfk.html

[T24] Swift：闭包
来源：http://hz.jinyuanbaomall.cn/gtxehaopuf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinqigfzy.top/gtvzifkfdy.html

[T25] Swift：结构体
来源：http://hz.yj20258888.top/gttocbihzt.html

struct P { var x: Int }
来源：http://hz.shzxlz.cn/gtrvsuwbik.html

[T26] Swift：类与重写
来源：http://hz.zhijiandao.cn/gtvcksqote.html

class A: Base { override func f() {} }
来源：http://hz.sweek.top/gtmodkaklz.html

[T27] Swift：错误处理
来源：http://hz.ydjk.org.cn/gtlmdiysst.html

do { try f() } catch { print(error) }
来源：http://hz.xuetiantiany.cn/gtkyhifuve.html

[T28] Swift：枚举
来源：http://hz.feifeiyinyue.top/gtnhjjnhky.html

enum Color { case red, green }
来源：http://hz.daria6918.cn/gtvbwbcvfl.html

[T29] Swift：guard 提前返回
来源：http://hz.zhongyouzk.top/gtgybmtjqa.html

guard let x = opt else { return }
来源：http://hz.vqdsnc.cn/gtyxtsxhqd.html

[T30] Swift：协议
来源：http://hz.52xcode.cn/gtruihnglk.html

protocol Shape { func area() -> Double }
来源：http://hz.gzhubu.top/gtwzrrlbdi.html

[T31] Lua：Hello World
来源：http://hz.nanxuanxn.top/gtknxwpnuu.html

print("Hello")
来源：http://hz.gzhubu.top/gtmarhtnta.html

[T32] Lua：局部变量
来源：http://hz.hongshengwenyu.top/gtwonirhlb.html

local a = 1
来源：http://hz.mhx1999.top/gtonoubcym.html

[T33] Lua：表（数组）
来源：http://hz.ydzc1.top/gthfovynke.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yvedp.cn/gtaovddsuw.html

[T34] Lua：遍历表
来源：http://hz.cashguo.top/gtnoomqhqf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.quarkkingdee.top/gtrfkqpgil.html

[T35] Lua：字典表
来源：http://hz.vqdsnc.cn/gtqogrcfzo.html

local d = { a = 1 };  d.b = 2
来源：http://hz.snrcjt.cn/gtmaaxclhr.html

[T36] Lua：函数
来源：http://hz.ydjk.org.cn/gtsubjmsgz.html

function add(a, b) return a + b end
来源：http://hz.yongpay.top/gtzpeepybw.html

[T37] Lua：字符串拼接
来源：http://hz.gotoacloud.top/gtkehvbvwz.html

"a" .. "b"
来源：http://hz.hywenlv.cn/gtqbftgszd.html

[T38] Lua：条件
来源：http://hz.zhoulong.xyz/gtevwkfquz.html

if x > 0 then print("正") end
来源：http://hz.sufxvd.cn/gtjpobxpwi.html

[T39] Lua：模式匹配
来源：http://hz.xylfe.cn/gtkwxsklet.html

string.find(s, "%d+")
来源：http://hz.dashuyun.cn/gtocoazieb.html

[T40] Lua：元表
来源：http://hz.redwolf501.top/gtmcmtflhe.html

setmetatable({}, { __index = base })
来源：http://hz.hnqzz.top/gtovqrdzai.html

[T41] Perl：Hello World
来源：http://hz.fzhhl.top/gtedfevzmm.html

print "Hello\n";
来源：http://hz.daxiang520.top/gtudwxutny.html

[T42] Perl：变量类型
来源：http://hz.hongshengwenyu.top/gtruajfkvt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.svipenyu.cn/gtkzaalvqu.html

[T43] Perl：字符串插值
来源：http://hz.svipenyu.cn/gtbgqotbgv.html

"值: $a"
来源：http://hz.kuanghao11.cn/gtbjreeznb.html

[T44] Perl：条件
来源：http://hz.zhaomingkeji.xyz/gtaqpfbwol.html

if ($a > 0) { print "正"; }
来源：http://hz.cqqwz.cn/gtgoirugwp.html

[T45] Perl：数组遍历
来源：http://hz.yanxiufei.cn/gtesebytgh.html

for my $x (@arr) { print $x; }
来源：http://hz.smart0.xyz/gtqgnxzvhl.html

[T46] Perl：哈希操作
来源：http://hz.ydjk.org.cn/gtwbzmnejh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yuanzhike.top/gtybeuzvct.html

[T47] Perl：正则捕获
来源：http://hz.hammf.cn/gttlnxrnxn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jyoumei.cn/gtimkigcfh.html

[T48] Perl：正则替换
来源：http://hz.0kj1m.cn/gtwtqynqzf.html

$s =~ s/old/new/g;
来源：http://hz.fzhhl.top/gtaqucrmkl.html

[T49] Perl：函数
来源：http://hz.yongpay.top/gtyygzptmz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhijiandao.cn/gtbfgwweoo.html

[T50] Perl：逐行读文件
来源：http://hz.xylfe.cn/gtwikftopv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cashguo.top/gtfiainumf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhaomingkeji.xyz/gtndsxoiog.html

[T51] Scala：Hello World
来源：http://hz.vqdsnc.cn/gthcaibrtt.html

println("Hello")
来源：http://hz.havefunace.top/gtdvcralfo.html

[T52] Scala：变量
来源：http://hz.dianchejie.cn/gtfxwzmkjx.html

val a = 1;  var b = 2
来源：http://hz.xinyue.icu/gtnoaetngn.html

[T53] Scala：字符串插值
来源：http://hz.sysykeji.top/gtmltleues.html

s"值: $b"
来源：http://hz.gzhubu.top/gtipvfexwl.html

[T54] Scala：集合映射
来源：http://hz.vqdsnc.cn/gtdbhydoxr.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.iojbl.cn/gtzuvajcbr.html

[T55] Scala：集合过滤
来源：http://hz.fzhhl.top/gtjicezmzn.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinghuilouyu.cn/gtlbfitzso.html

[T56] Scala：样例类
来源：http://hz.pycfn.com/gtgnngnpth.html

case class User(name: String, age: Int)
来源：http://hz.feifeiyinyue.top/gtrjtrjlhx.html

[T57] Scala：模式匹配
来源：http://hz.aizwys.cn/gtyocogjad.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhoulong.xyz/gtblfzayph.html

[T58] Scala：函数定义
来源：http://hz.daria6918.cn/gttcciawug.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.snrcjt.cn/gtvbtktfyp.html

[T59] Scala：循环
来源：http://hz.daxiang520.top/gtbraxnmms.html

for (i <- 1 to 10) println(i)
来源：http://hz.gzhubu.top/gtqennfwwy.html

[T60] Scala：折叠
来源：http://hz.c1oappe.top/gtudggsrmq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.nanxuanxn.top/gtgljmdzox.html

================================================================================
来源：http://hz.iojbl.cn/gtfwccpmyi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.havefunace.top/gtjrxllylg.html

================================================================================
来源：http://hz.jqgufenzy.top/gtexlvocsr.html

[U01] Py：创建虚拟环境
来源：http://hz.hywenlv.cn/gtjjfgpomv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yanxiufei.cn/gtdlmrpxzv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.52xcode.cn/gtwyowtrbw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shanyushiyangkeji.top/gtsdvwhfkp.html

[U03] Py：加载 .env 配置
来源：http://hz.jinqigfzy.top/gtjsxvldno.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hnxiangtu.top/gtrthesyqs.html

[U04] Py：变量调试打印
来源：http://hz.zhaomingkeji.xyz/gtowdfqzyr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258888.top/gtpjuyvnsn.html

[U05] Py：列表去重且保序
来源：http://hz.hnqzz.top/gtmitoqzwi.html

list(dict.fromkeys(arr))
来源：http://hz.yongpay.top/gttetghhrq.html

[U06] Py：合并两个字典
来源：http://hz.52xcode.cn/gtcwzhkrcd.html

{**a, **b}
来源：http://hz.cqqwz.cn/gtocoyaepr.html

[U07] Py：反转字典键值
来源：http://hz.dashuyun.cn/gtlqbytpow.html

{v: k for k, v in d.items()}
来源：http://hz.hywenlv.cn/gtjhhuzivf.html

[U08] Py：展平二维列表
来源：http://hz.gogol.net.cn/gtfbbabcgl.html

[y for x in nested for y in x]
来源：http://hz.xuanzx.com/gtrwnleuzp.html

[U09] Py：字典取最大值的键
来源：http://hz.mhx1999.top/gtgysfrgmm.html

max(d, key=d.get)
来源：http://hz.mhx1999.top/gtcjxcuidq.html

[U10] Py：按值排序字典
来源：http://hz.sysykeji.top/gtqasnvblu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sufxvd.cn/gtjjarwxrc.html

[U11] Py：生成器表达式
来源：http://hz.sxryk.cn/gtozuawwat.html

(x * 2 for x in arr)
来源：http://hz.meibo888.top/gtvrtsavjt.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tanke756.top/gtzgadttpt.html

Counter(arr).most_common(3)
来源：http://hz.cucudq.cn/gtyarakfkd.html

[U13] Py：固定长度队列
来源：http://hz.52xcode.cn/gtjbjwvlmq.html

deque(maxlen=10)
来源：http://hz.zhijiandao.cn/gtiydjhklx.html

[U14] Py：分组收集到列表
来源：http://hz.jinqigfzy.top/gtqohsuwzy.html

defaultdict(list)
来源：http://hz.ywan-chungtsiang.top/gtoxzbggld.html

[U15] Py：高精度计时
来源：http://hz.tanke756.top/gttlnvimuu.html

t = time.perf_counter()
来源：http://hz.ydzc1.top/gtrdxhsyke.html

[U16] Py：命令行参数解析
来源：http://hz.svipenyu.cn/gtpuzjeewn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zycfv.cn/gtrzmieezb.html

[U17] Py：初始化日志
来源：http://hz.jqgfzy.top/gtgkquxfmq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ywan-chungtsiang.top/gtxaepfsqk.html

[U18] Py：预编译正则
来源：http://hz.jyoumei.cn/gtyxopiupu.html

pat = re.compile(r"\d+")
来源：http://hz.zhaomingkeji.xyz/gtwhwkwlmm.html

[U19] Py：正则替换带回调
来源：http://hz.yvedp.cn/gtgswfsgvr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhiwuduotai.top/gtdyusrqqj.html

[U20] Py：缓存函数结果
来源：http://hz.jinqigfzy.top/gtybfgvcow.html

@functools.lru_cache(maxsize=None)
来源：http://hz.316326.xyz/gtriyactkr.html

[U21] Py：自定义上下文管理器
来源：http://hz.yonumen.top/gtwfblbxoy.html

@contextlib.contextmanager
来源：http://hz.svipenyu.cn/gtlylvuclv.html

[U22] Py：矩阵转置
来源：http://hz.tanke756.top/gtegaowkbl.html

list(zip(*m))
来源：http://hz.shangyingyoupin.top/gtewcdaqdm.html

[U23] Py：分块读取大文件
来源：http://hz.ydjk.org.cn/gtqakbfgtk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.fzhhl.top/gtfwsappsd.html

[U24] Py：路径操作
来源：http://hz.zhijiandao.cn/gtdflmabka.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.nanxinkj.top/gttkvewhdy.html

[U25] Py：CSV 按字典读
来源：http://hz.nanxuanxn.top/gtogwzlbhu.html

csv.DictReader(f)
来源：http://hz.sweek.top/gtiklzqpcb.html

[U26] Py：并发下载
来源：http://hz.cucudq.cn/gtttiqvaly.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ydjk.org.cn/gtkutlcejr.html

[U27] Py：异步 HTTP
来源：http://hz.zdqjudy.top/gtuwttqsic.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shanyushiyangtech.top/gtwnautpwu.html

[U28] Py：类型别名
来源：http://hz.snrcjt.cn/gtjokboecr.html

UserId = int
来源：http://hz.ydjk.org.cn/gtuffbvqhe.html

[U29] Py：属性校验
来源：http://hz.nanxinkj.top/gtelxafpls.html

@property 与 @x.setter 配合
来源：http://hz.ehwqpu.com/gtnohsosmp.html

[U30] Py：数据类
来源：http://hz.yangfankeji.com/gtdsrzczew.html

@dataclass(slots=True)
来源：http://hz.shanyushiyangtech.top/gtvbpfbrjx.html

[U31] Py：单测
来源：http://hz.meibo888.top/gtncwpndbb.html

python -m pytest -q
来源：http://hz.jinyuanbaomall.cn/gtbibvlelz.html

[U32] Py：代码格式化
来源：http://hz.zhixingplan.top/gtajppnfgf.html

ruff format . && ruff check --fix .
来源：http://hz.wangshuangyany.cn/gtjandfdvf.html

[U33] Py：打包发布
来源：http://hz.guannengcc.top/gtflrkxbvd.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.quarkkingdee.top/gttuprfjvk.html

[U34] Py：判断编码
来源：http://hz.yongpay.top/gtkoqzalyg.html

chardet.detect(raw)
来源：http://hz.9152youxi.cn/gtvqjqhqmo.html

[U35] Py：发送邮件
来源：http://hz.cheryme.top/gtjwylrwmy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cashguo.top/gtfzokauis.html

[U36] Py：定时任务
来源：http://hz.zycfv.cn/gtvysyizbb.html

schedule.every(10).minutes.do(job)
来源：http://hz.xuanzx.com/gtfbenllkv.html

[U37] Py：读写 Excel
来源：http://hz.tianlin.xyz/gtgdvgjsed.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yuanzhike.top/gtgxwnqdie.html

[U38] Py：获取脚本所在目录
来源：http://hz.jqgfzy.top/gtjgucqzdc.html

Path(__file__).resolve().parent
来源：http://hz.0kj1m.cn/gtlxaxgrmt.html

[U39] Py：判断是否在交互环境
来源：http://hz.sysykeji.top/gtojezabup.html

sys.stdout.isatty()
来源：http://hz.vqdsnc.cn/gtzwywyktv.html

[U40] Py：打印到标准错误
来源：http://hz.ywan-chungtsiang.top/gtulhhtlpq.html

print("err", file=sys.stderr)
来源：http://hz.wangdashe.top/gtsceilggk.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhongyouzk.top/gthazlaxfv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.gzhubu.top/gtmvyseapr.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ivvv.top/gthnlndody.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shangyingyoupin.top/gtrkpoxmfi.html

[U43] PHP：声明命名空间
来源：http://hz.vqdsnc.cn/gtrdpoqnda.html

namespace App\Http;
来源：http://hz.xylfe.cn/gtcbirsagv.html

[U44] PHP：开启严格类型
来源：http://hz.sysykeji.top/gtvshajyjp.html

declare(strict_types=1);
来源：http://hz.sufxvd.cn/gtnrjpuerg.html

[U45] PHP：类型声明与返回类型
来源：http://hz.fengsongda.top/gtommjwjqb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuxming.cn/gtkjvrtjqx.html

[U46] PHP：可空类型
来源：http://hz.cucudq.cn/gtnwsynufy.html

?string $name = null
来源：http://hz.xinyue.icu/gtpctdxxgw.html

[U47] PHP：联合类型
来源：http://hz.shuidangran.top/gtvmzwlbby.html

int|string $id
来源：http://hz.cucudq.cn/gtznkfaclm.html

[U48] PHP：纯枚举
来源：http://hz.c1oappe.top/gtkwwcwtja.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.andypj.xyz/gtyoyansfc.html

[U49] PHP：只读属性
来源：http://hz.xinyue.icu/gtnuswlcms.html

public readonly string $name
来源：http://hz.jlsjyb.cn/gttbnbavte.html

[U50] PHP：构造器属性提升
来源：http://hz.mhx1999.top/gtndvedbdh.html

public function __construct(private int $id) {}
来源：http://hz.ppjwa.cn/gtqijcpqyb.html

[U51] PHP：数组解构
来源：http://hz.hywenlv.cn/gtpgekqauh.html

[$a, $b] = $arr;
来源：http://hz.daxiang520.top/gthqpwxxnn.html

[U52] PHP：箭头函数
来源：http://hz.jqgfzy.top/gtlghxnjgu.html

$double = fn($x) => $x * 2;
来源：http://hz.sufxvd.cn/gtdoydgzzp.html

[U53] PHP：空合并运算符
来源：http://hz.316326.xyz/gtgkumgnfs.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhaomingkeji.xyz/gtvqbyyxiq.html

[U54] PHP：空安全调用
来源：http://hz.ybcxt.top/gttjbqaqgx.html

$obj?->method()
来源：http://hz.guannengcc.top/gtcibpjjjr.html

[U55] PHP：match 表达式
来源：http://hz.zhaomingkeji.xyz/gttcwpbasd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shanyushiyangkeji.top/gtrtbxzadb.html

[U56] PHP：命名参数
来源：http://hz.sufxvd.cn/gthmabjdha.html

f(a: 1, b: 2)
来源：http://hz.meibo888.top/gtlvcqrtap.html

[U57] PHP：字符串插值
来源：http://hz.bjfxy.top/gtlpozmuud.html

"值: {$a}"
来源：http://hz.cdnleiting.top/gtvrhdpgas.html

[U58] PHP：数组三件套
来源：http://hz.quarkkingdee.top/gtuwixkswu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yangfankeji.com/gtlerietwb.html

[U59] PHP：自定义排序
来源：http://hz.xuanzx.com/gtdjxalxmw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guowangkeji.top/gtcgyofctg.html

[U60] PHP：JSON 编解码
来源：http://hz.jinyuanbaomall.cn/gtgdphgssv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.kuanghao11.cn/gtlheolama.html

[U61] PHP：正则
来源：http://hz.xinyue.icu/gtztdarnrw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.dianchejie.cn/gtnrhnebxd.html

[U62] PHP：日期对象
来源：http://hz.tian-w.cn/gtlmxapxkx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yuxming.cn/gtoswhflwa.html

[U63] PHP：文件读写
来源：http://hz.yuanzhike.top/gtgwwguoxa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.aizwys.cn/gtasyfmzvh.html

[U64] PHP：目录遍历
来源：http://hz.ywan-chungtsiang.top/gtxqlqgpes.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.aizwys.cn/gthtjcfghl.html

[U65] PHP：会话
来源：http://hz.daria6918.cn/gticwwqula.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.tian-w.cn/gtoeudhakn.html

[U66] PHP：设置 Cookie
来源：http://hz.wangdashe.top/gtdteixplf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.fengsongda.top/gtyeuehpkm.html

[U67] PHP：处理文件上传
来源：http://hz.jianghu66.top/gtqcaqmjhr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yanxiufei.cn/gtabxwcyik.html

[U68] PHP：PDO 连接
来源：http://hz.ywan-chungtsiang.top/gtcwcvzxlc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ppjwa.cn/gtcnkkjosh.html

[U69] PHP：PDO 预处理
来源：http://hz.zhijiandao.cn/gtgfuvwwoq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xinyue.icu/gtomdbskov.html

[U70] PHP：PDO 事务
来源：http://hz.yonumen.top/gtvuylllzu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.daxiang520.top/gtoqqxyiqd.html


<!-- 参考信息 -->