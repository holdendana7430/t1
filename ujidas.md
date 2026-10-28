代发 wailian999

[S45] C++：lambda
来源：http://hz.xylfe.cn/gtlboyehxc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xziqi.cn/gtsqeyvkrw.html

[S46] C++：函数模板
来源：http://hz.jqgufenzy.top/gtgfduvgau.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenzaomai.com/gtaxdiqqig.html

[S47] C++：结构化绑定遍历
来源：http://hz.jqgufenzy.top/gtexbkbimk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.andypj.xyz/gtaqpgxjpy.html

[S48] C++：逐行读文件
来源：http://hz.zhongyouzk.top/gtaqxruytb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sweek.top/gtxrexrhxd.html

while (std::getline(in, line)) { }
来源：http://hz.jinyuanbaomall.cn/gtqauucavf.html

[S49] C++：写文件
来源：http://hz.zycfv.cn/gtmgqppixs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhongyouzk.top/gtepzqprrd.html

[S50] C++：格式化数字
来源：http://hz.hysaishi.cn/gtssgmqadr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigfzy.top/gtyntcrbqj.html

[S51] C++：显式类型转换
来源：http://hz.sysykeji.top/gtbzftgnlq.html

static_cast<double>(a) / b
来源：http://hz.dashuyun.cn/gtvqsqwcah.html

[S52] C++：const 与 noexcept
来源：http://hz.jinqigufen.top/gtiuqjsbno.html

int size() const noexcept { return n_; }
来源：http://hz.yvedp.cn/gtlkglkftp.html

[S53] C++：移动语义
来源：http://hz.havefunace.top/gtpoohdcwi.html

std::vector<int> w = std::move(v);
来源：http://hz.316326.xyz/gtbtoehtts.html

[S54] C++：异常处理
来源：http://hz.vqdsnc.cn/gtfyymndcj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.bjfxy.top/gtmdvqpixi.html

[S55] C++：结构化绑定
来源：http://hz.jinqigfzy.top/gtjwogcxjp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ivvv.top/gtmxoatkzh.html

[S56] C++：optional
来源：http://hz.ydjk.org.cn/gtaggbplvc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yueranfly.top/gtqrnvrfhu.html

[S57] C++：编译期常量
来源：http://hz.feifeiyinyue.top/gtgkbsaapc.html

constexpr int N = 10;
来源：http://hz.zhixingplan.top/gtgoxumeke.html

[S58] C++：命名空间
来源：http://hz.jinyuanbaomall.cn/gtzjsyqkeg.html

namespace ns { int f() { return 1; } }
来源：http://hz.aizwys.cn/gtnsiwyodo.html

[S59] C++：静态断言
来源：http://hz.pengpengdd.cyou/gttjypsizx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hongshengwenyu.top/gtbguwldgn.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangkeji.top/gtlxuiihdu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigufen.top/gtkneqjlqe.html

================================================================================
来源：http://hz.aizwys.cn/gtepwzmvsi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.bjfxy.top/gtujqmiaip.html

================================================================================
来源：http://hz.guannengcc.top/gtyudlqptq.html

[T01] Kotlin：Hello World
来源：http://hz.xuanzx.com/gtgloqwmwm.html

println("Hello")
来源：http://hz.sxryk.cn/gtwaooutjw.html

[T02] Kotlin：变量
来源：http://hz.xylfe.cn/gtnirrmyoi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aibaodan.cn/gtljcfxmbb.html

[T03] Kotlin：字符串模板
来源：http://hz.shangyingyoupin.top/gtnuibxkby.html

"值: $b"
来源：http://hz.hammf.cn/gtbmovnxdh.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangtech.top/gtzycsjaxb.html

val n: String? = null;  n?.length
来源：http://hz.jyoumei.cn/gteiefgojo.html

[T05] Kotlin：when 表达式
来源：http://hz.cucudq.cn/gtinchkuvj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.daxiang520.top/gtfxkcxvyh.html

[T06] Kotlin：集合映射
来源：http://hz.nanxinkj.top/gthbrjxbxn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shzxlz.cn/gtkfrxpqkd.html

[T07] Kotlin：集合过滤
来源：http://hz.zdqjudy.top/gtganbiwtn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xingfuxueyuan.xyz/gtyfxtoewg.html

[T08] Kotlin：数据类
来源：http://hz.jqgufenzy.top/gtrjufvveu.html

data class User(val name: String, val age: Int)
来源：http://hz.316326.xyz/gtnlctcukx.html

[T09] Kotlin：扩展函数
来源：http://hz.sysykeji.top/gtfkkztfdn.html

fun String.exclaim() = this + "!"
来源：http://hz.hysaishi.cn/gtbchcbjwu.html

[T10] Kotlin：默认参数
来源：http://hz.yj20258.top/gtowcybrjr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yuanzhike.top/gtvcwrikdb.html

[T11] Kotlin：协程
来源：http://hz.gotoacloud.top/gttyhqeowf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sweek.top/gtdrbmqesx.html

[T12] Kotlin：解构声明
来源：http://hz.zhongyouzk.top/gtdlajnxer.html

val (a, b) = Pair(1, 2)
来源：http://hz.xuanzx.com/gtoalpnkcf.html

[T13] Kotlin：只读 Map
来源：http://hz.dianchejie.cn/gtajjvwczi.html

val m = mapOf("a" to 1)
来源：http://hz.pengpengdd.cyou/gtygvpftmo.html

[T14] Kotlin：循环
来源：http://hz.kuanghao11.cn/gtybshxpsj.html

for (i in 1..10) println(i)
来源：http://hz.9152youxi.cn/gtrdlqzftu.html

[T15] Kotlin：接口
来源：http://hz.feifeiyinyue.top/gtvjpddctm.html

interface Shape { fun area(): Double }
来源：http://hz.zhixingplan.top/gtmxnisxkw.html

[T16] Swift：Hello World
来源：http://hz.jyoumei.cn/gtiboqtsqu.html

print("Hello")
来源：http://hz.zdqjudy.top/gtrnezjpjs.html

[T17] Swift：变量与常量
来源：http://hz.gzhubu.top/gtznvsravy.html

var a = 1;  let b = 2
来源：http://hz.cashguo.top/gtqswgnbvb.html

[T18] Swift：字符串插值
来源：http://hz.9152youxi.cn/gthzrbiosg.html

"值: \(b)"
来源：http://hz.yanxiufei.cn/gtlvizmroa.html

[T19] Swift：可选绑定
来源：http://hz.dashuyun.cn/gtqvvjtgwl.html

if let n = opt { print(n) }
来源：http://hz.hammf.cn/gteyzokzmb.html

[T20] Swift：数组操作
来源：http://hz.nwbrower.top/gtwvyhihkv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yanxiufei.cn/gtarqmfhbr.html

[T21] Swift：遍历
来源：http://hz.nanxinkj.top/gtoswlkvhx.html

for x in a { print(x) }
来源：http://hz.9152youxi.cn/gtpaitkgln.html

[T22] Swift：字典
来源：http://hz.kuanghao11.cn/gtqzdwfoik.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhoulong.xyz/gtzgpzodnk.html

[T23] Swift：函数
来源：http://hz.sweek.top/gtqrbusreg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.guowangkeji.top/gtmunldshc.html

[T24] Swift：闭包
来源：http://hz.jlsjyb.cn/gtlryykaph.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.redwolf501.top/gtcdcpwnrl.html

[T25] Swift：结构体
来源：http://hz.mhx1999.top/gtvoozfnzn.html

struct P { var x: Int }
来源：http://hz.52xcode.cn/gtzxtzpumx.html

[T26] Swift：类与重写
来源：http://hz.nanxinkj.top/gtrkqwcdlk.html

class A: Base { override func f() {} }
来源：http://hz.fengsongda.top/gtlqcwrxpg.html

[T27] Swift：错误处理
来源：http://hz.zhixingplan.top/gtphwnfjei.html

do { try f() } catch { print(error) }
来源：http://hz.xuetiantiany.cn/gtkohkzvld.html

[T28] Swift：枚举
来源：http://hz.guannengcc.top/gtigfowtlm.html

enum Color { case red, green }
来源：http://hz.ydzc1.top/gtrcrdcsam.html

[T29] Swift：guard 提前返回
来源：http://hz.yanxiufei.cn/gttdbchwrz.html

guard let x = opt else { return }
来源：http://hz.cashguo.top/gtafktrnyf.html

[T30] Swift：协议
来源：http://hz.yj20258888.top/gtycfkofhh.html

protocol Shape { func area() -> Double }
来源：http://hz.yj20258888.top/gtqpcneiop.html

[T31] Lua：Hello World
来源：http://hz.chenjidiqi.icu/gtuhsbegxl.html

print("Hello")
来源：http://hz.iojbl.cn/gtzqmziibo.html

[T32] Lua：局部变量
来源：http://hz.yanxiufei.cn/gtqhzhoooq.html

local a = 1
来源：http://hz.yj20258.top/gtglkuhthy.html

[T33] Lua：表（数组）
来源：http://hz.cucudq.cn/gtxkghzygy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangdashe.top/gtyunfeqni.html

[T34] Lua：遍历表
来源：http://hz.jqgufenzy.top/gtvijxjgdw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.havefunace.top/gtcecsoojk.html

[T35] Lua：字典表
来源：http://hz.jianghu66.top/gtgmfdjudn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xuanzx.com/gtnimymtgj.html

[T36] Lua：函数
来源：http://hz.zycfv.cn/gtutodwkat.html

function add(a, b) return a + b end
来源：http://hz.jqgufenzy.top/gtpbexzetg.html

[T37] Lua：字符串拼接
来源：http://hz.xziqi.cn/gtvzewlrzh.html

"a" .. "b"
来源：http://hz.hfpthk.cn/gtdmaqcgwv.html

[T38] Lua：条件
来源：http://hz.aizwys.cn/gtfdekxwba.html

if x > 0 then print("正") end
来源：http://hz.chenzaomai.com/gtfxcetdmv.html

[T39] Lua：模式匹配
来源：http://hz.hysaishi.cn/gtlcsoabyr.html

string.find(s, "%d+")
来源：http://hz.sysykeji.top/gtmtyliats.html

[T40] Lua：元表
来源：http://hz.ydzc1.top/gtqetmxqli.html

setmetatable({}, { __index = base })
来源：http://hz.ybcxt.top/gtqaduvzat.html

[T41] Perl：Hello World
来源：http://hz.9152youxi.cn/gtjkrmfmrk.html

print "Hello\n";
来源：http://hz.ehwqpu.com/gtbdpjodvi.html

[T42] Perl：变量类型
来源：http://hz.jlsjyb.cn/gtfynmkowc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xuetiantiany.cn/gtpvlohqzz.html

[T43] Perl：字符串插值
来源：http://hz.bjfxy.top/gtlxrzqfyn.html

"值: $a"
来源：http://hz.nanxinkj.top/gtvgvvsjkb.html

[T44] Perl：条件
来源：http://hz.yonumen.top/gttiznceom.html

if ($a > 0) { print "正"; }
来源：http://hz.ehwqpu.com/gtgxzrmwzn.html

[T45] Perl：数组遍历
来源：http://hz.zhaomingkeji.xyz/gtbkhwfmwh.html

for my $x (@arr) { print $x; }
来源：http://hz.cheryme.top/gthyitqonq.html

[T46] Perl：哈希操作
来源：http://hz.ybcxt.top/gttgezvhlu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.fzhhl.top/gtdryopefm.html

[T47] Perl：正则捕获
来源：http://hz.hywenlv.cn/gtaplxxlix.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jiagoushi.top/gtjoifqtva.html

[T48] Perl：正则替换
来源：http://hz.fzhhl.top/gtshzjvila.html

$s =~ s/old/new/g;
来源：http://hz.fengsongda.top/gtdtrnxmyk.html

[T49] Perl：函数
来源：http://hz.jinghuilouyu.cn/gtlfzkjmgt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sweek.top/gttdwfprnu.html

[T50] Perl：逐行读文件
来源：http://hz.gotoacloud.top/gtxqmxxdkd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.redwolf501.top/gttohypomj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.daxiang520.top/gtongdczhu.html

[T51] Scala：Hello World
来源：http://hz.wangshuangyany.cn/gtzrhdoxdh.html

println("Hello")
来源：http://hz.fzhhl.top/gtiroqceef.html

[T52] Scala：变量
来源：http://hz.ivvv.top/gtinhhwoue.html

val a = 1;  var b = 2
来源：http://hz.chenzaomai.com/gtzmdzhapi.html

[T53] Scala：字符串插值
来源：http://hz.xuanzx.com/gtwkjpschd.html

s"值: $b"
来源：http://hz.zhaomingkeji.xyz/gtixgfeitw.html

[T54] Scala：集合映射
来源：http://hz.guowangkeji.top/gtjtpjstpc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sufxvd.cn/gtegmitkck.html

[T55] Scala：集合过滤
来源：http://hz.yueranfly.top/gtdmtiltqp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydjk.org.cn/gtpnpsityj.html

[T56] Scala：样例类
来源：http://hz.jlsjyb.cn/gtsrybncat.html

case class User(name: String, age: Int)
来源：http://hz.daria6918.cn/gtgpoovrkw.html

[T57] Scala：模式匹配
来源：http://hz.sufxvd.cn/gtjgsmjdlc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hysaishi.cn/gtvgkoorgg.html

[T58] Scala：函数定义
来源：http://hz.hysaishi.cn/gtqrtmgjyz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.vqdsnc.cn/gtfduhhmlg.html

[T59] Scala：循环
来源：http://hz.sysykeji.top/gtcdmrgjuz.html

for (i <- 1 to 10) println(i)
来源：http://hz.sweek.top/gtgvapkwdc.html

[T60] Scala：折叠
来源：http://hz.zhengqikj.top/gtymhwkraa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hywenlv.cn/gtyfoomsug.html

================================================================================
来源：http://hz.bjfxy.top/gtpwdfqryu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cucudq.cn/gtgapourqf.html

================================================================================
来源：http://hz.nanxinkj.top/gtlrmcyiuq.html

[U01] Py：创建虚拟环境
来源：http://hz.shanyushiyangtech.top/gtnocqomqc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jinghuilouyu.cn/gtsbigptfe.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sysykeji.top/gtkjdglncx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.316326.xyz/gtcyrrmzfc.html

[U03] Py：加载 .env 配置
来源：http://hz.aizwys.cn/gtkfiydabb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.bjfxy.top/gtoostyyyt.html

[U04] Py：变量调试打印
来源：http://hz.zhijiandao.cn/gtqcpquhiq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cdnleiting.top/gthfkfhige.html

[U05] Py：列表去重且保序
来源：http://hz.bjfxy.top/gtqbyjssjw.html

list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gtdxefwrgz.html

[U06] Py：合并两个字典
来源：http://hz.yanxiufei.cn/gtclnjpagl.html

{**a, **b}
来源：http://hz.jianghu66.top/gtkoneiwxk.html

[U07] Py：反转字典键值
来源：http://hz.cqqwz.cn/gtkluxsehb.html

{v: k for k, v in d.items()}
来源：http://hz.aibaodan.cn/gtatlqbaqo.html

[U08] Py：展平二维列表
来源：http://hz.yuxming.cn/gtsnuwpoeq.html

[y for x in nested for y in x]
来源：http://hz.svipenyu.cn/gtoyuwnube.html

[U09] Py：字典取最大值的键
来源：http://hz.cheryme.top/gtyylkqeed.html

max(d, key=d.get)
来源：http://hz.snrcjt.cn/gtwhhupqyv.html

[U10] Py：按值排序字典
来源：http://hz.fzhhl.top/gtbtkvyejs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.guowangkeji.top/gtgtbqsozz.html

[U11] Py：生成器表达式
来源：http://hz.wangshuangyany.cn/gtuxoublwv.html

(x * 2 for x in arr)
来源：http://hz.yvedp.cn/gtxchdxirf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhijiandao.cn/gtlwsmuhmw.html

Counter(arr).most_common(3)
来源：http://hz.mhx1999.top/gtzpjpcqbr.html

[U13] Py：固定长度队列
来源：http://hz.yj202588.top/gtmpmhklcq.html

deque(maxlen=10)
来源：http://hz.316326.xyz/gthvqdloxj.html

[U14] Py：分组收集到列表
来源：http://hz.zdqjudy.top/gtzmebnoew.html

defaultdict(list)
来源：http://hz.chenlongwang.top/gtbkjkhwvq.html

[U15] Py：高精度计时
来源：http://hz.pycfn.com/gtcxqxvwbp.html

t = time.perf_counter()
来源：http://hz.zhoulong.xyz/gtwfmuvxel.html

[U16] Py：命令行参数解析
来源：http://hz.xuanzx.com/gttorltbjv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.316326.xyz/gthtzjqgyu.html

[U17] Py：初始化日志
来源：http://hz.vqdsnc.cn/gtckylnrzo.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.mhx1999.top/gtpxvaqznx.html

[U18] Py：预编译正则
来源：http://hz.zycfv.cn/gtclnzxbba.html

pat = re.compile(r"\d+")
来源：http://hz.dashuyun.cn/gtfiyliwgu.html

[U19] Py：正则替换带回调
来源：http://hz.cashguo.top/gtrgbwxdfy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ybcxt.top/gtgfebpdvk.html

[U20] Py：缓存函数结果
来源：http://hz.hysaishi.cn/gtpzqotgek.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhiwuduotai.top/gtwrilgfqf.html

[U21] Py：自定义上下文管理器
来源：http://hz.ydjk.org.cn/gtykqmzijl.html

@contextlib.contextmanager
来源：http://hz.wangshuangyany.cn/gtadvxrrrc.html

[U22] Py：矩阵转置
来源：http://hz.kuanghao11.cn/gtbujhhzga.html

list(zip(*m))
来源：http://hz.zhoulong.xyz/gtbaeozvci.html

[U23] Py：分块读取大文件
来源：http://hz.gotoacloud.top/gtruvsaspl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hywenlv.cn/gtzqihoygt.html

[U24] Py：路径操作
来源：http://hz.ydjk.org.cn/gthjtnxzdh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gaohongyu789.top/gttknpjcme.html

[U25] Py：CSV 按字典读
来源：http://hz.yuanzhike.top/gtkhxzdnzv.html

csv.DictReader(f)
来源：http://hz.fengsongda.top/gtxsjaydwa.html

[U26] Py：并发下载
来源：http://hz.hywenlv.cn/gthprslnay.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zycfv.cn/gtlbhuajji.html

[U27] Py：异步 HTTP
来源：http://hz.ppjwa.cn/gtcxcdvcfz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.smart0.xyz/gtpyiqczin.html

[U28] Py：类型别名
来源：http://hz.dianchejie.cn/gtvugsppdo.html

UserId = int
来源：http://hz.chenjidiqi.icu/gtbyuqvxhu.html

[U29] Py：属性校验
来源：http://hz.meibo888.top/gtwhpaxwdd.html

@property 与 @x.setter 配合
来源：http://hz.mhx1999.top/gthzfeazlp.html

[U30] Py：数据类
来源：http://hz.yueranfly.top/gtdsciqigd.html

@dataclass(slots=True)
来源：http://hz.guowangkeji.top/gtkzmjhlyf.html

[U31] Py：单测
来源：http://hz.nanxinkj.top/gtblxusily.html

python -m pytest -q
来源：http://hz.zhoulong.xyz/gtaegpdbxb.html

[U32] Py：代码格式化
来源：http://hz.dianchejie.cn/gtonpjxevx.html

ruff format . && ruff check --fix .
来源：http://hz.dianchejie.cn/gtvrzfsnju.html

[U33] Py：打包发布
来源：http://hz.ybcxt.top/gtgfbdyenv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.dianchejie.cn/gtbmprpxyf.html

[U34] Py：判断编码
来源：http://hz.birdmap.top/gtnfuvsons.html

chardet.detect(raw)
来源：http://hz.zhongyouzk.top/gtbehildpn.html

[U35] Py：发送邮件
来源：http://hz.chenzaomai.com/gthvpvywtq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hnxiangtu.top/gtccyjlsds.html

[U36] Py：定时任务
来源：http://hz.zhengqikj.top/gtcngkdoih.html

schedule.every(10).minutes.do(job)
来源：http://hz.yongpay.top/gtzxaaxihm.html

[U37] Py：读写 Excel
来源：http://hz.kuanghao11.cn/gtywnjswfj.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xziqi.cn/gtutyniqkx.html

[U38] Py：获取脚本所在目录
来源：http://hz.hfpthk.cn/gtnjiksdrx.html

Path(__file__).resolve().parent
来源：http://hz.feifeiyinyue.top/gtyumupwhp.html

[U39] Py：判断是否在交互环境
来源：http://hz.jinghuilouyu.cn/gtblyjuekv.html

sys.stdout.isatty()
来源：http://hz.yanxiufei.cn/gtelepsnzx.html

[U40] Py：打印到标准错误
来源：http://hz.xuanzx.com/gtlkddrixz.html

print("err", file=sys.stderr)
来源：http://hz.tian-w.cn/gtawoomblf.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.guannengcc.top/gttusisnlh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shanyushiyangtech.top/gtgzdxillc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.havefunace.top/gtojztuggu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.guannengcc.top/gtsxjwpmgs.html

[U43] PHP：声明命名空间
来源：http://hz.jyoumei.cn/gtlqvyuhlz.html

namespace App\Http;
来源：http://hz.ydjk.org.cn/gtxcdepawq.html

[U44] PHP：开启严格类型
来源：http://hz.wangdashe.top/gtiiabztzs.html

declare(strict_types=1);
来源：http://hz.cdnleiting.top/gtazryhwxb.html

[U45] PHP：类型声明与返回类型
来源：http://hz.feifeiyinyue.top/gtodgvrxpr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jianghu66.top/gtspruvztv.html

[U46] PHP：可空类型
来源：http://hz.9152youxi.cn/gtqectbvnw.html

?string $name = null
来源：http://hz.xziqi.cn/gtcakkuext.html

[U47] PHP：联合类型
来源：http://hz.daxiang520.top/gtwongqiss.html

int|string $id
来源：http://hz.shanyushiyangkeji.top/gtmrzermen.html

[U48] PHP：纯枚举
来源：http://hz.yueranfly.top/gtujpghtyu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jianghu66.top/gtvhzmtzbs.html

[U49] PHP：只读属性
来源：http://hz.shanyushiyangtech.top/gtsrxlswtq.html

public readonly string $name
来源：http://hz.xylfe.cn/gttaiqmawi.html

[U50] PHP：构造器属性提升
来源：http://hz.316326.xyz/gtqvnsiwlg.html

public function __construct(private int $id) {}
来源：http://hz.yj20258888.top/gtyxqtlflq.html

[U51] PHP：数组解构
来源：http://hz.yuxming.cn/gtyesoysvx.html

[$a, $b] = $arr;
来源：http://hz.fzhhl.top/gtgtujebnr.html

[U52] PHP：箭头函数
来源：http://hz.yj202588.top/gtsdvjvlcd.html

$double = fn($x) => $x * 2;
来源：http://hz.sxryk.cn/gtmefqjlrh.html

[U53] PHP：空合并运算符
来源：http://hz.shzxlz.cn/gtdqetatfh.html

$v = $a ?? $b ?? "default";
来源：http://hz.smart0.xyz/gtdoabmuyt.html

[U54] PHP：空安全调用
来源：http://hz.fengsongda.top/gtondkmyzf.html

$obj?->method()
来源：http://hz.dianchejie.cn/gtouzhmmfs.html

[U55] PHP：match 表达式
来源：http://hz.nanxinkj.top/gtqxurmwqm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cucudq.cn/gtordxssrr.html

[U56] PHP：命名参数
来源：http://hz.nanxuanxn.top/gtxpkbfqyj.html

f(a: 1, b: 2)
来源：http://hz.dashuyun.cn/gtgbutujmy.html

[U57] PHP：字符串插值
来源：http://hz.sufxvd.cn/gtgzbjnesv.html

"值: {$a}"
来源：http://hz.hnqzz.top/gtdfrrajdj.html

[U58] PHP：数组三件套
来源：http://hz.haohaochexian.top/gtszlysabg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.tianlin.xyz/gtufbodqah.html

[U59] PHP：自定义排序
来源：http://hz.yongpay.top/gtoehwxuds.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.andypj.xyz/gtjgfhvjnj.html

[U60] PHP：JSON 编解码
来源：http://hz.jinghuilouyu.cn/gtcznqvoqs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jqgfzy.top/gtmyjeasmj.html

[U61] PHP：正则
来源：http://hz.andypj.xyz/gtwmnwsvwi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xylfe.cn/gtxfetovag.html

[U62] PHP：日期对象
来源：http://hz.0kj1m.cn/gthqddtygg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhongyouzk.top/gtrjkqwgdz.html

[U63] PHP：文件读写
来源：http://hz.xingfuxueyuan.xyz/gtxvdemujf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinghuilouyu.cn/gtvgmrprpd.html

[U64] PHP：目录遍历
来源：http://hz.hfpthk.cn/gtlsqxnpev.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ydzc1.top/gtqrzjqlju.html

[U65] PHP：会话
来源：http://hz.jqgufenzy.top/gtcogomxsl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.tanke756.top/gtwcjlelnr.html

[U66] PHP：设置 Cookie
来源：http://hz.wangshuangyany.cn/gtvlqjjmkq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.0kj1m.cn/gtgphopdnz.html

[U67] PHP：处理文件上传
来源：http://hz.yongpay.top/gtbugmstte.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhongyouzk.top/gtaedscquh.html

[U68] PHP：PDO 连接
来源：http://hz.hnxiangtu.top/gtahyhrfpw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.nanxuanxn.top/gtscolikab.html

[U69] PHP：PDO 预处理
来源：http://hz.xinyue.icu/gtfrispstr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.snrcjt.cn/gtqwenmzlj.html

[U70] PHP：PDO 事务
来源：http://hz.kuanghao11.cn/gtntpncvgo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zycfv.cn/gtgyslphdr.html


<!-- 参考信息 -->