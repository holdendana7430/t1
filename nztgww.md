代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://hz.0kj1m.cn/gthcnwjmtp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258888.top/gtpnyzkfun.html

[S48] C++：逐行读文件
来源：http://hz.sysykeji.top/gtllofsrlm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.andypj.xyz/gtndemzrhk.html

while (std::getline(in, line)) { }
来源：http://hz.jinqigfzy.top/gtgoyynbtb.html

[S49] C++：写文件
来源：http://hz.cucudq.cn/gtcarpache.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yanxiufei.cn/gteqfiphys.html

[S50] C++：格式化数字
来源：http://hz.nanxuanxn.top/gtntudfall.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jqgufenzy.top/gtdolazwhw.html

[S51] C++：显式类型转换
来源：http://hz.xingfuxueyuan.xyz/gtrpxjwcdk.html

static_cast<double>(a) / b
来源：http://hz.jinghuilouyu.cn/gteehimiwu.html

[S52] C++：const 与 noexcept
来源：http://hz.hnqzz.top/gtatqrxlvp.html

int size() const noexcept { return n_; }
来源：http://hz.cdnleiting.top/gteddooerm.html

[S53] C++：移动语义
来源：http://hz.ehwqpu.com/gtcdrisgua.html

std::vector<int> w = std::move(v);
来源：http://hz.c1oappe.top/gtlfuqtlhh.html

[S54] C++：异常处理
来源：http://hz.havefunace.top/gtdtoiahpr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xinyue.icu/gtbxkhmcil.html

[S55] C++：结构化绑定
来源：http://hz.xuetiantiany.cn/gtkpyeeqoh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yueranfly.top/gtimpiovgs.html

[S56] C++：optional
来源：http://hz.shuidangran.top/gtgytshbhq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tianlin.xyz/gtcoodtlxa.html

[S57] C++：编译期常量
来源：http://hz.aizwys.cn/gtfrqwwdbw.html

constexpr int N = 10;
来源：http://hz.jianghu66.top/gtodypxtvl.html

[S58] C++：命名空间
来源：http://hz.gotoacloud.top/gtllfzfsqx.html

namespace ns { int f() { return 1; } }
来源：http://hz.mhx1999.top/gttaznnvlv.html

[S59] C++：静态断言
来源：http://hz.tanke756.top/gtoafpszmk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.bjfxy.top/gtwzesznkq.html

[S60] C++：遍历并删除元素
来源：http://hz.xziqi.cn/gtphfsvftu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.316326.xyz/gtbydmjytj.html

================================================================================
来源：http://hz.aizwys.cn/gtygnimnxb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhiwuduotai.top/gtxddjjzwl.html

================================================================================
来源：http://hz.nanxinkj.top/gtjfjfhfjh.html

[T01] Kotlin：Hello World
来源：http://hz.wangshuangyany.cn/gtvipfxxdf.html

println("Hello")
来源：http://hz.chenzaomai.com/gtbwudbnjz.html

[T02] Kotlin：变量
来源：http://hz.cashguo.top/gtbususmzi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.havefunace.top/gtqarrpgvl.html

[T03] Kotlin：字符串模板
来源：http://hz.wangdashe.top/gtgibgqbvl.html

"值: $b"
来源：http://hz.jqgfzy.top/gtftbhufzz.html

[T04] Kotlin：空安全
来源：http://hz.birdmap.top/gtpzxyrvpr.html

val n: String? = null;  n?.length
来源：http://hz.xuetiantiany.cn/gtdbjbdzrp.html

[T05] Kotlin：when 表达式
来源：http://hz.hammf.cn/gtuoyyaooq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zdqjudy.top/gtqfaaxntm.html

[T06] Kotlin：集合映射
来源：http://hz.kuanghao11.cn/gtlacekbxl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shuidangran.top/gtgjtluewb.html

[T07] Kotlin：集合过滤
来源：http://hz.nwbrower.top/gtoukjushh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnxiangtu.top/gtxhrmwjgl.html

[T08] Kotlin：数据类
来源：http://hz.fzhhl.top/gtxwxpqsru.html

data class User(val name: String, val age: Int)
来源：http://hz.shzxlz.cn/gtuckmmaxx.html

[T09] Kotlin：扩展函数
来源：http://hz.hongshengwenyu.top/gteusbtawq.html

fun String.exclaim() = this + "!"
来源：http://hz.meibo888.top/gtpmsggjyv.html

[T10] Kotlin：默认参数
来源：http://hz.hnqzz.top/gtrjlnrcsp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aizwys.cn/gtozbjpygk.html

[T11] Kotlin：协程
来源：http://hz.jqgfzy.top/gtumxyntrs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tianlin.xyz/gtsjkydobr.html

[T12] Kotlin：解构声明
来源：http://hz.shangyingyoupin.top/gttsrijzmk.html

val (a, b) = Pair(1, 2)
来源：http://hz.haohaochexian.top/gtytcfhhuj.html

[T13] Kotlin：只读 Map
来源：http://hz.tianlin.xyz/gtwqxapwnq.html

val m = mapOf("a" to 1)
来源：http://hz.dashuyun.cn/gtqagahxvn.html

[T14] Kotlin：循环
来源：http://hz.guannengcc.top/gtapjjaxbw.html

for (i in 1..10) println(i)
来源：http://hz.gzhubu.top/gtqycvbxzu.html

[T15] Kotlin：接口
来源：http://hz.aibaodan.cn/gtiahjyese.html

interface Shape { fun area(): Double }
来源：http://hz.chenzaomai.com/gtvdzbncvv.html

[T16] Swift：Hello World
来源：http://hz.wangdashe.top/gtfxzbpvdt.html

print("Hello")
来源：http://hz.pengpengdd.cyou/gtafmxvcwu.html

[T17] Swift：变量与常量
来源：http://hz.fzhhl.top/gttlzqupcf.html

var a = 1;  let b = 2
来源：http://hz.yongpay.top/gtjgzdysdr.html

[T18] Swift：字符串插值
来源：http://hz.zhaomingkeji.xyz/gttwwtsbel.html

"值: \(b)"
来源：http://hz.zhoulong.xyz/gtcuimcvsp.html

[T19] Swift：可选绑定
来源：http://hz.zhengqikj.top/gtqqnhthik.html

if let n = opt { print(n) }
来源：http://hz.mhx1999.top/gtkhcuiqsa.html

[T20] Swift：数组操作
来源：http://hz.jinghuilouyu.cn/gteznpcgaz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cashguo.top/gtbkwzcrzg.html

[T21] Swift：遍历
来源：http://hz.gotoacloud.top/gtilzsmoyi.html

for x in a { print(x) }
来源：http://hz.yangfankeji.com/gtkngxehkv.html

[T22] Swift：字典
来源：http://hz.cheryme.top/gtlgirlcof.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sxryk.cn/gtzuuteoje.html

[T23] Swift：函数
来源：http://hz.jyoumei.cn/gtkqftofix.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hnxiangtu.top/gtkbgfqmzp.html

[T24] Swift：闭包
来源：http://hz.guowangkeji.top/gttcgabbwz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.andypj.xyz/gtclltldrc.html

[T25] Swift：结构体
来源：http://hz.ydjk.org.cn/gthhaqhcdj.html

struct P { var x: Int }
来源：http://hz.feifeiyinyue.top/gtayangbls.html

[T26] Swift：类与重写
来源：http://hz.hongshengwenyu.top/gtobmceckt.html

class A: Base { override func f() {} }
来源：http://hz.gotoacloud.top/gtimvusrej.html

[T27] Swift：错误处理
来源：http://hz.dashuyun.cn/gtvqgyvgly.html

do { try f() } catch { print(error) }
来源：http://hz.pycfn.com/gtqaxiedqp.html

[T28] Swift：枚举
来源：http://hz.yonumen.top/gtmvodzyos.html

enum Color { case red, green }
来源：http://hz.jianghu66.top/gtmrvvoins.html

[T29] Swift：guard 提前返回
来源：http://hz.chenjidiqi.icu/gttwoeumkd.html

guard let x = opt else { return }
来源：http://hz.hysaishi.cn/gtzckgobij.html

[T30] Swift：协议
来源：http://hz.kuanghao11.cn/gteruukdzc.html

protocol Shape { func area() -> Double }
来源：http://hz.zhengqikj.top/gtzbjsxhko.html

[T31] Lua：Hello World
来源：http://hz.yueranfly.top/gtedfsllyt.html

print("Hello")
来源：http://hz.yuxming.cn/gtephptshw.html

[T32] Lua：局部变量
来源：http://hz.nanxuanxn.top/gtlsgxjqwb.html

local a = 1
来源：http://hz.shanyushiyangtech.top/gtrgpwcnmb.html

[T33] Lua：表（数组）
来源：http://hz.haohaochexian.top/gtosncmlyv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.daxiang520.top/gtptisbvgq.html

[T34] Lua：遍历表
来源：http://hz.guowangkeji.top/gtggigzkph.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gaohongyu789.top/gtaimefjsg.html

[T35] Lua：字典表
来源：http://hz.daxiang520.top/gtiswzbkfn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj20258888.top/gtwvzbaakt.html

[T36] Lua：函数
来源：http://hz.cdnleiting.top/gtjgdcsxxl.html

function add(a, b) return a + b end
来源：http://hz.nanxuanxn.top/gtxeiavvbm.html

[T37] Lua：字符串拼接
来源：http://hz.yuxming.cn/gtrtvgcrgv.html

"a" .. "b"
来源：http://hz.nanxuanxn.top/gtpouscfzx.html

[T38] Lua：条件
来源：http://hz.iojbl.cn/gtpstvmyst.html

if x > 0 then print("正") end
来源：http://hz.zhixingplan.top/gttdviqpzf.html

[T39] Lua：模式匹配
来源：http://hz.shanyushiyangtech.top/gtprmuszem.html

string.find(s, "%d+")
来源：http://hz.sufxvd.cn/gttugjqdbd.html

[T40] Lua：元表
来源：http://hz.mhx1999.top/gtlqrksgjg.html

setmetatable({}, { __index = base })
来源：http://hz.aizwys.cn/gticpjoevm.html

[T41] Perl：Hello World
来源：http://hz.0kj1m.cn/gthgawdozl.html

print "Hello\n";
来源：http://hz.yuxming.cn/gtlakbielb.html

[T42] Perl：变量类型
来源：http://hz.haohaochexian.top/gteegfviss.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jyoumei.cn/gtgqxskgof.html

[T43] Perl：字符串插值
来源：http://hz.gogol.net.cn/gtfdylyngz.html

"值: $a"
来源：http://hz.yj20258.top/gtiiednvoc.html

[T44] Perl：条件
来源：http://hz.jianghu66.top/gttnpdpwdy.html

if ($a > 0) { print "正"; }
来源：http://hz.yvedp.cn/gtnpexbcgb.html

[T45] Perl：数组遍历
来源：http://hz.redwolf501.top/gticwskzfk.html

for my $x (@arr) { print $x; }
来源：http://hz.316326.xyz/gtnubtcfnc.html

[T46] Perl：哈希操作
来源：http://hz.jinghuilouyu.cn/gtegmoseri.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xuanzx.com/gtlbwugetp.html

[T47] Perl：正则捕获
来源：http://hz.yj20258888.top/gtfwdnhaof.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hammf.cn/gtbgixrova.html

[T48] Perl：正则替换
来源：http://hz.yongpay.top/gtcdsxfcjc.html

$s =~ s/old/new/g;
来源：http://hz.xingfuxueyuan.xyz/gtmxhgzcab.html

[T49] Perl：函数
来源：http://hz.tanke756.top/gttyvmkxxp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cashguo.top/gtqjljpeuj.html

[T50] Perl：逐行读文件
来源：http://hz.hongshengwenyu.top/gtkjccjber.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenjidiqi.icu/gtdspclmuf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ywan-chungtsiang.top/gtxmphuayk.html

[T51] Scala：Hello World
来源：http://hz.hnxiangtu.top/gtjrthcbav.html

println("Hello")
来源：http://hz.hysaishi.cn/gtbiywnkgv.html

[T52] Scala：变量
来源：http://hz.fengsongda.top/gtsblpbzkh.html

val a = 1;  var b = 2
来源：http://hz.ydzc1.top/gtmssvyuwg.html

[T53] Scala：字符串插值
来源：http://hz.zhijiandao.cn/gtbyzvzvhu.html

s"值: $b"
来源：http://hz.hfpthk.cn/gtqbdtmhky.html

[T54] Scala：集合映射
来源：http://hz.yangfankeji.com/gtswgaimus.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shanyushiyangkeji.top/gtpvujrqet.html

[T55] Scala：集合过滤
来源：http://hz.yvedp.cn/gthdaqlxje.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ivvv.top/gtbnjohrdc.html

[T56] Scala：样例类
来源：http://hz.hammf.cn/gtynziywco.html

case class User(name: String, age: Int)
来源：http://hz.shzxlz.cn/gtqoprqvkq.html

[T57] Scala：模式匹配
来源：http://hz.zdqjudy.top/gtrrdtsfpm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yj20258888.top/gtgaebdjda.html

[T58] Scala：函数定义
来源：http://hz.yj20258.top/gtqzffpish.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.birdmap.top/gtrtcpnwco.html

[T59] Scala：循环
来源：http://hz.sysykeji.top/gtdpryvdhz.html

for (i <- 1 to 10) println(i)
来源：http://hz.meibo888.top/gtvkajzpvk.html

[T60] Scala：折叠
来源：http://hz.52xcode.cn/gtkkypksjs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.haohaochexian.top/gthyufxemu.html

================================================================================
来源：http://hz.zdqjudy.top/gtidmodzmr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnxiangtu.top/gtfaorevth.html

================================================================================
来源：http://hz.cucudq.cn/gttpwwiuif.html

[U01] Py：创建虚拟环境
来源：http://hz.guannengcc.top/gtwlfgrhla.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.gogol.net.cn/gtlfwywqoh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cucudq.cn/gtldvwlgqg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yueranfly.top/gtwpjznmco.html

[U03] Py：加载 .env 配置
来源：http://hz.smart0.xyz/gtdyqzueht.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yongpay.top/gtqrwrhbdm.html

[U04] Py：变量调试打印
来源：http://hz.fzhhl.top/gtdovwsmlp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xziqi.cn/gtbecanqau.html

[U05] Py：列表去重且保序
来源：http://hz.sysykeji.top/gtbifzvlfq.html

list(dict.fromkeys(arr))
来源：http://hz.gzhubu.top/gtuxqezqef.html

[U06] Py：合并两个字典
来源：http://hz.feifeiyinyue.top/gtxzyljaxh.html

{**a, **b}
来源：http://hz.guowangkeji.top/gtfhtcjios.html

[U07] Py：反转字典键值
来源：http://hz.ehwqpu.com/gtxvrruodf.html

{v: k for k, v in d.items()}
来源：http://hz.gaohongyu789.top/gtuuawcddg.html

[U08] Py：展平二维列表
来源：http://hz.9152youxi.cn/gtnsarudpl.html

[y for x in nested for y in x]
来源：http://hz.jqgfzy.top/gtkijmjdns.html

[U09] Py：字典取最大值的键
来源：http://hz.cashguo.top/gtlfpxitin.html

max(d, key=d.get)
来源：http://hz.shuidangran.top/gtrpxwrbuo.html

[U10] Py：按值排序字典
来源：http://hz.gaohongyu789.top/gtqjhwaeke.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sufxvd.cn/gtjakdkatt.html

[U11] Py：生成器表达式
来源：http://hz.mhx1999.top/gtotuvvtsf.html

(x * 2 for x in arr)
来源：http://hz.cashguo.top/gtuevrenin.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zdqjudy.top/gtbmcoaygg.html

Counter(arr).most_common(3)
来源：http://hz.aibaodan.cn/gtgxtfhcoz.html

[U13] Py：固定长度队列
来源：http://hz.daxiang520.top/gtemslflhs.html

deque(maxlen=10)
来源：http://hz.hfpthk.cn/gtrquanwzn.html

[U14] Py：分组收集到列表
来源：http://hz.redwolf501.top/gtuemdxcjv.html

defaultdict(list)
来源：http://hz.ivvv.top/gtkpkewuyo.html

[U15] Py：高精度计时
来源：http://hz.cashguo.top/gtauhdlsvh.html

t = time.perf_counter()
来源：http://hz.guannengcc.top/gtwoswwtgv.html

[U16] Py：命令行参数解析
来源：http://hz.chenzaomai.com/gtgefanmju.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.shanyushiyangkeji.top/gthywuxdak.html

[U17] Py：初始化日志
来源：http://hz.tanke756.top/gtdhsxlunq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.quarkkingdee.top/gtlnueocrz.html

[U18] Py：预编译正则
来源：http://hz.cheryme.top/gtnrxnftyq.html

pat = re.compile(r"\d+")
来源：http://hz.sweek.top/gtparkbuer.html

[U19] Py：正则替换带回调
来源：http://hz.yj202588.top/gtpchbqadr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.guowangkeji.top/gtapagkeoa.html

[U20] Py：缓存函数结果
来源：http://hz.mhx1999.top/gtofyrdwas.html

@functools.lru_cache(maxsize=None)
来源：http://hz.svipenyu.cn/gtqrslvevv.html

[U21] Py：自定义上下文管理器
来源：http://hz.shuidangran.top/gtxvsanqin.html

@contextlib.contextmanager
来源：http://hz.cucudq.cn/gtknihcchh.html

[U22] Py：矩阵转置
来源：http://hz.ppjwa.cn/gtufrqholk.html

list(zip(*m))
来源：http://hz.shuidangran.top/gteruhqytd.html

[U23] Py：分块读取大文件
来源：http://hz.cucudq.cn/gtujsfxrni.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jqgufenzy.top/gtukanrbfr.html

[U24] Py：路径操作
来源：http://hz.cashguo.top/gtnqwlsavq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yuxming.cn/gtquoqrdyi.html

[U25] Py：CSV 按字典读
来源：http://hz.gogol.net.cn/gtmpmippsy.html

csv.DictReader(f)
来源：http://hz.yangfankeji.com/gtbzisxyvf.html

[U26] Py：并发下载
来源：http://hz.tianlin.xyz/gtnovuyalw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.daria6918.cn/gtswerqhnt.html

[U27] Py：异步 HTTP
来源：http://hz.tian-w.cn/gtawmbckyl.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhengqikj.top/gtckcnguhm.html

[U28] Py：类型别名
来源：http://hz.xziqi.cn/gtzwndfnzs.html

UserId = int
来源：http://hz.0kj1m.cn/gtoqfcbcsp.html

[U29] Py：属性校验
来源：http://hz.yj202588.top/gtmhgsjfgl.html

@property 与 @x.setter 配合
来源：http://hz.xylfe.cn/gtiaapbwtf.html

[U30] Py：数据类
来源：http://hz.yj202588.top/gtcbyzqqlg.html

@dataclass(slots=True)
来源：http://hz.daxiang520.top/gtpuefiawt.html

[U31] Py：单测
来源：http://hz.daria6918.cn/gtampboodc.html

python -m pytest -q
来源：http://hz.jqgfzy.top/gtgcrrgqeu.html

[U32] Py：代码格式化
来源：http://hz.cucudq.cn/gtchpectyu.html

ruff format . && ruff check --fix .
来源：http://hz.jinqigufen.top/gtmkflniwh.html

[U33] Py：打包发布
来源：http://hz.jqgfzy.top/gtrwlqgavc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yj20258.top/gtgvevcnkg.html

[U34] Py：判断编码
来源：http://hz.hnxiangtu.top/gtidpezoxt.html

chardet.detect(raw)
来源：http://hz.0kj1m.cn/gtyzphuqbe.html

[U35] Py：发送邮件
来源：http://hz.hywenlv.cn/gtqrqxpbce.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jlsjyb.cn/gtfkkrlagp.html

[U36] Py：定时任务
来源：http://hz.chenjidiqi.icu/gtkiguyqqs.html

schedule.every(10).minutes.do(job)
来源：http://hz.cheryme.top/gtosdtgtjd.html

[U37] Py：读写 Excel
来源：http://hz.zhaomingkeji.xyz/gtdwviufzh.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xingfuxueyuan.xyz/gtgujdcyzr.html

[U38] Py：获取脚本所在目录
来源：http://hz.zdqjudy.top/gtelsstvlr.html

Path(__file__).resolve().parent
来源：http://hz.xylfe.cn/gtjmlyqdgu.html

[U39] Py：判断是否在交互环境
来源：http://hz.meibo888.top/gtmvaiyruj.html

sys.stdout.isatty()
来源：http://hz.hongshengwenyu.top/gtzxabzyin.html

[U40] Py：打印到标准错误
来源：http://hz.yongpay.top/gtvzzasoyq.html

print("err", file=sys.stderr)
来源：http://hz.tian-w.cn/gtepvpietq.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.iojbl.cn/gtmdfmsqst.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.fzhhl.top/gtycfwthsw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.cucudq.cn/gtqdlpvgla.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yvedp.cn/gtqrzphmuq.html

[U43] PHP：声明命名空间
来源：http://hz.xylfe.cn/gtdiijocnm.html

namespace App\Http;
来源：http://hz.nanxinkj.top/gtjukmoysm.html

[U44] PHP：开启严格类型
来源：http://hz.zdqjudy.top/gtnosxguil.html

declare(strict_types=1);
来源：http://hz.snrcjt.cn/gtmciqbuxu.html

[U45] PHP：类型声明与返回类型
来源：http://hz.gogol.net.cn/gtlpnfyoss.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtkuminzbn.html

[U46] PHP：可空类型
来源：http://hz.zhiwuduotai.top/gtjbnfdhad.html

?string $name = null
来源：http://hz.guannengcc.top/gtztiyrcun.html

[U47] PHP：联合类型
来源：http://hz.sweek.top/gtdniklzpn.html

int|string $id
来源：http://hz.yvedp.cn/gtdbsbijni.html

[U48] PHP：纯枚举
来源：http://hz.redwolf501.top/gtycdgxflb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.chenjidiqi.icu/gtvyvzqexp.html

[U49] PHP：只读属性
来源：http://hz.haohaochexian.top/gtggwewwsb.html

public readonly string $name
来源：http://hz.tianlin.xyz/gttzbywlkz.html

[U50] PHP：构造器属性提升
来源：http://hz.cucudq.cn/gtunlzoydl.html

public function __construct(private int $id) {}
来源：http://hz.sxryk.cn/gtovlwpadj.html

[U51] PHP：数组解构
来源：http://hz.guannengcc.top/gtjjkvbaqj.html

[$a, $b] = $arr;
来源：http://hz.hfpthk.cn/gtymajkciq.html

[U52] PHP：箭头函数
来源：http://hz.hfpthk.cn/gtsgkztyae.html

$double = fn($x) => $x * 2;
来源：http://hz.xinyue.icu/gtrjeazeke.html

[U53] PHP：空合并运算符
来源：http://hz.jianghu66.top/gtfhzegjbd.html

$v = $a ?? $b ?? "default";
来源：http://hz.sweek.top/gtoeunuelu.html

[U54] PHP：空安全调用
来源：http://hz.zhixingplan.top/gtqlvxhuie.html

$obj?->method()
来源：http://hz.52xcode.cn/gtrzpyhato.html

[U55] PHP：match 表达式
来源：http://hz.cheryme.top/gtouzebjir.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj20258888.top/gtmllfugjf.html

[U56] PHP：命名参数
来源：http://hz.yuxming.cn/gtpvyziizf.html

f(a: 1, b: 2)
来源：http://hz.redwolf501.top/gtenfwzjod.html

[U57] PHP：字符串插值
来源：http://hz.tianlin.xyz/gtwdwkrnbm.html

"值: {$a}"
来源：http://hz.xuanzx.com/gtlljsdmmi.html

[U58] PHP：数组三件套
来源：http://hz.jlsjyb.cn/gtkcbzmbsf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hnqzz.top/gttghisvbf.html

[U59] PHP：自定义排序
来源：http://hz.yvedp.cn/gtzhmwqwvl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtowmomohr.html

[U60] PHP：JSON 编解码
来源：http://hz.cdnleiting.top/gtohmfzhjg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xylfe.cn/gtouucguti.html

[U61] PHP：正则
来源：http://hz.chenlongwang.top/gtpgbjghod.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhaomingkeji.xyz/gtrmoynxrt.html

[U62] PHP：日期对象
来源：http://hz.sufxvd.cn/gtjoaarisr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cashguo.top/gtjiccdrev.html

[U63] PHP：文件读写
来源：http://hz.yanxiufei.cn/gtgssirpae.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zdqjudy.top/gtryfbgiqo.html

[U64] PHP：目录遍历
来源：http://hz.vqdsnc.cn/gtxdwzblmu.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jqgfzy.top/gtebkgvnrn.html

[U65] PHP：会话
来源：http://hz.zhaomingkeji.xyz/gtqlwaqqwf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shzxlz.cn/gthjrelwui.html

[U66] PHP：设置 Cookie
来源：http://hz.andypj.xyz/gttxyyqjnm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gogol.net.cn/gtwcjeovqp.html

[U67] PHP：处理文件上传
来源：http://hz.zhoulong.xyz/gtisnkyemc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jqgfzy.top/gtpkwpnfje.html

[U68] PHP：PDO 连接
来源：http://hz.zhengqikj.top/gtjwokkfob.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.pycfn.com/gtwevtwasq.html

[U69] PHP：PDO 预处理
来源：http://hz.sxryk.cn/gttpbwtfmb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jinqigfzy.top/gtgawldkbv.html

[U70] PHP：PDO 事务
来源：http://hz.shanyushiyangkeji.top/gtyjgatlso.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.chenzaomai.com/gtrzwxmxff.html

[U71] PHP：抛出异常
来源：http://hz.quarkkingdee.top/gthzrtrhsz.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhiwuduotai.top/gtgbgzpqwt.html

[U72] PHP：写错误日志
来源：http://hz.jlsjyb.cn/gtujsyrccf.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhijiandao.cn/gtxvahuctv.html


<!-- 参考信息 -->