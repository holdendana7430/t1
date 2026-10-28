代发 wailian999

int size() const noexcept { return n_; }
来源：http://hz.nwbrower.top/gtwrhxbjhr.html

[S53] C++：移动语义
来源：http://hz.yueranfly.top/gtipojhuew.html

std::vector<int> w = std::move(v);
来源：http://hz.dianchejie.cn/gtpbiythgk.html

[S54] C++：异常处理
来源：http://hz.c1oappe.top/gtgsmxsbrw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cheryme.top/gtnzgytmxx.html

[S55] C++：结构化绑定
来源：http://hz.birdmap.top/gtylroutla.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.haohaochexian.top/gtdiixeunl.html

[S56] C++：optional
来源：http://hz.zhijiandao.cn/gtqndajfmh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnqzz.top/gtvxgbdeck.html

[S57] C++：编译期常量
来源：http://hz.yj202588.top/gtbtvqvzva.html

constexpr int N = 10;
来源：http://hz.zycfv.cn/gtiptsbawm.html

[S58] C++：命名空间
来源：http://hz.xinyue.icu/gtrhfiuody.html

namespace ns { int f() { return 1; } }
来源：http://hz.quarkkingdee.top/gtsjfrqcmf.html

[S59] C++：静态断言
来源：http://hz.daria6918.cn/gtzpvifbcd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhijiandao.cn/gtyujfcete.html

[S60] C++：遍历并删除元素
来源：http://hz.xuetiantiany.cn/gticxabqft.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shangyingyoupin.top/gtzaevlmcz.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtbzvqjtcd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pycfn.com/gtfxlalmbs.html

================================================================================
来源：http://hz.cheryme.top/gtqmlpuspg.html

[T01] Kotlin：Hello World
来源：http://hz.hnxiangtu.top/gtxammjnqr.html

println("Hello")
来源：http://hz.pengpengdd.cyou/gtimgdlsbv.html

[T02] Kotlin：变量
来源：http://hz.ppjwa.cn/gtxmaqsxkp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.birdmap.top/gtqsdpgfnz.html

[T03] Kotlin：字符串模板
来源：http://hz.pengpengdd.cyou/gttpdntlzb.html

"值: $b"
来源：http://hz.shangyingyoupin.top/gtlyngebhb.html

[T04] Kotlin：空安全
来源：http://hz.jlsjyb.cn/gtkiayhsql.html

val n: String? = null;  n?.length
来源：http://hz.andypj.xyz/gttlsgsbjh.html

[T05] Kotlin：when 表达式
来源：http://hz.nwbrower.top/gtxlfhodpb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jlsjyb.cn/gtvqqsjnxb.html

[T06] Kotlin：集合映射
来源：http://hz.aibaodan.cn/gtywfwzqvd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnqzz.top/gtjarmyhxb.html

[T07] Kotlin：集合过滤
来源：http://hz.ehwqpu.com/gtrboypavd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xinyue.icu/gtyvsnrbkf.html

[T08] Kotlin：数据类
来源：http://hz.feifeiyinyue.top/gtedzzuylz.html

data class User(val name: String, val age: Int)
来源：http://hz.bjfxy.top/gtpndfxbhv.html

[T09] Kotlin：扩展函数
来源：http://hz.zhaomingkeji.xyz/gtppfbozix.html

fun String.exclaim() = this + "!"
来源：http://hz.sysykeji.top/gtxkvmjcnt.html

[T10] Kotlin：默认参数
来源：http://hz.hnqzz.top/gtaokzljcq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.tianlin.xyz/gtzkmutleh.html

[T11] Kotlin：协程
来源：http://hz.gzhubu.top/gtgfbijawv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gzhubu.top/gtjaotonef.html

[T12] Kotlin：解构声明
来源：http://hz.mhx1999.top/gttmredcid.html

val (a, b) = Pair(1, 2)
来源：http://hz.quarkkingdee.top/gtcbcglqmj.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtlhfyyqlq.html

val m = mapOf("a" to 1)
来源：http://hz.fengsongda.top/gtiimilbhp.html

[T14] Kotlin：循环
来源：http://hz.52xcode.cn/gthsvhaeyu.html

for (i in 1..10) println(i)
来源：http://hz.hnxiangtu.top/gtdtwcyhoj.html

[T15] Kotlin：接口
来源：http://hz.ppjwa.cn/gtyxueshsq.html

interface Shape { fun area(): Double }
来源：http://hz.snrcjt.cn/gtxjaqbmev.html

[T16] Swift：Hello World
来源：http://hz.yuxming.cn/gtudheqkay.html

print("Hello")
来源：http://hz.shanyushiyangtech.top/gtyvgkagtw.html

[T17] Swift：变量与常量
来源：http://hz.0kj1m.cn/gttpaowjxc.html

var a = 1;  let b = 2
来源：http://hz.meibo888.top/gtdnbrmlpq.html

[T18] Swift：字符串插值
来源：http://hz.svipenyu.cn/gtfkrsgdmw.html

"值: \(b)"
来源：http://hz.ybcxt.top/gtyavprrvp.html

[T19] Swift：可选绑定
来源：http://hz.svipenyu.cn/gtoqyzauds.html

if let n = opt { print(n) }
来源：http://hz.xuetiantiany.cn/gtjivytcog.html

[T20] Swift：数组操作
来源：http://hz.jlsjyb.cn/gtqrdvpwrz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.vqdsnc.cn/gtrjxkbvcl.html

[T21] Swift：遍历
来源：http://hz.ppjwa.cn/gtklljwzxx.html

for x in a { print(x) }
来源：http://hz.hysaishi.cn/gtxqbquuqv.html

[T22] Swift：字典
来源：http://hz.birdmap.top/gtynmdvbgi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xziqi.cn/gtxzuzromh.html

[T23] Swift：函数
来源：http://hz.pycfn.com/gtphgvgifx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shanyushiyangtech.top/gtwwpmxbfp.html

[T24] Swift：闭包
来源：http://hz.zhiwuduotai.top/gtnfxpyvsk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tanke756.top/gtwtbmgsfq.html

[T25] Swift：结构体
来源：http://hz.xziqi.cn/gtyfwtejio.html

struct P { var x: Int }
来源：http://hz.guannengcc.top/gtqqcywyxz.html

[T26] Swift：类与重写
来源：http://hz.meibo888.top/gtkochmyzr.html

class A: Base { override func f() {} }
来源：http://hz.ybcxt.top/gtemdtsmbj.html

[T27] Swift：错误处理
来源：http://hz.yuxming.cn/gtliwjodgr.html

do { try f() } catch { print(error) }
来源：http://hz.jlsjyb.cn/gtqggzmbgx.html

[T28] Swift：枚举
来源：http://hz.kuanghao11.cn/gtnulnnevm.html

enum Color { case red, green }
来源：http://hz.zhoulong.xyz/gtizmyjmcp.html

[T29] Swift：guard 提前返回
来源：http://hz.smart0.xyz/gtzxxlhtsb.html

guard let x = opt else { return }
来源：http://hz.daxiang520.top/gtusxlidji.html

[T30] Swift：协议
来源：http://hz.hongshengwenyu.top/gtudjavejf.html

protocol Shape { func area() -> Double }
来源：http://hz.chenzaomai.com/gtrvawzxad.html

[T31] Lua：Hello World
来源：http://hz.hywenlv.cn/gtbibbnsrv.html

print("Hello")
来源：http://hz.dashuyun.cn/gttczqlbdn.html

[T32] Lua：局部变量
来源：http://hz.pycfn.com/gtzzqhsrcw.html

local a = 1
来源：http://hz.xuetiantiany.cn/gtmaxrkzyl.html

[T33] Lua：表（数组）
来源：http://hz.dianchejie.cn/gtgnetnhoi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cheryme.top/gtvyddwvhj.html

[T34] Lua：遍历表
来源：http://hz.yj202588.top/gtejlvvule.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.birdmap.top/gtmkmgqlaz.html

[T35] Lua：字典表
来源：http://hz.zycfv.cn/gtwtpjxqar.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shanyushiyangkeji.top/gtiujwsivk.html

[T36] Lua：函数
来源：http://hz.xinyue.icu/gtzesyyjcq.html

function add(a, b) return a + b end
来源：http://hz.yuxming.cn/gtqnplatrg.html

[T37] Lua：字符串拼接
来源：http://hz.sxryk.cn/gtvvxbihuv.html

"a" .. "b"
来源：http://hz.gaohongyu789.top/gtnujtxgzq.html

[T38] Lua：条件
来源：http://hz.bjfxy.top/gtzzpdgily.html

if x > 0 then print("正") end
来源：http://hz.zhijiandao.cn/gtlwicjgcr.html

[T39] Lua：模式匹配
来源：http://hz.hongshengwenyu.top/gtwrshqnfo.html

string.find(s, "%d+")
来源：http://hz.nwbrower.top/gtiaucxoct.html

[T40] Lua：元表
来源：http://hz.feifeiyinyue.top/gtbostjwub.html

setmetatable({}, { __index = base })
来源：http://hz.zdqjudy.top/gtgelbjure.html

[T41] Perl：Hello World
来源：http://hz.guowangkeji.top/gtmyapnwhn.html

print "Hello\n";
来源：http://hz.xinyue.icu/gtgesbpqth.html

[T42] Perl：变量类型
来源：http://hz.zycfv.cn/gtzffmzvlu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.redwolf501.top/gthhmsulfo.html

[T43] Perl：字符串插值
来源：http://hz.nanxinkj.top/gtrtrqsrym.html

"值: $a"
来源：http://hz.jinqigufen.top/gthderxpdb.html

[T44] Perl：条件
来源：http://hz.daxiang520.top/gtdqkiwpna.html

if ($a > 0) { print "正"; }
来源：http://hz.9152youxi.cn/gtvjhgajdo.html

[T45] Perl：数组遍历
来源：http://hz.vqdsnc.cn/gtilwpming.html

for my $x (@arr) { print $x; }
来源：http://hz.chenlongwang.top/gtegvcvcdt.html

[T46] Perl：哈希操作
来源：http://hz.cdnleiting.top/gtzbneulhr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gaohongyu789.top/gtacvgzcog.html

[T47] Perl：正则捕获
来源：http://hz.chenlongwang.top/gtucemwtib.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.tian-w.cn/gtbtobenjf.html

[T48] Perl：正则替换
来源：http://hz.ppjwa.cn/gtjgczdxyk.html

$s =~ s/old/new/g;
来源：http://hz.xuetiantiany.cn/gtnqhlxhyp.html

[T49] Perl：函数
来源：http://hz.cheryme.top/gtwzxircmo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtpzbfuotc.html

[T50] Perl：逐行读文件
来源：http://hz.yangfankeji.com/gtncmxvebq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhijiandao.cn/gtvrjxkwlq.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.aibaodan.cn/gtsounvhvk.html

[T51] Scala：Hello World
来源：http://hz.yuxming.cn/gtffdfcwtp.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gtikjhuzhx.html

[T52] Scala：变量
来源：http://hz.tanke756.top/gtwskffcph.html

val a = 1;  var b = 2
来源：http://hz.zhixingplan.top/gtoifdvapy.html

[T53] Scala：字符串插值
来源：http://hz.jianghu66.top/gtuxatrera.html

s"值: $b"
来源：http://hz.guowangkeji.top/gtmjmkasrr.html

[T54] Scala：集合映射
来源：http://hz.jlsjyb.cn/gtefvmufix.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jiagoushi.top/gtefzbmjcl.html

[T55] Scala：集合过滤
来源：http://hz.yj202588.top/gtookvdpag.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.nwbrower.top/gtqhwlmnmo.html

[T56] Scala：样例类
来源：http://hz.hammf.cn/gtadnmabyt.html

case class User(name: String, age: Int)
来源：http://hz.shanyushiyangtech.top/gtndzjhgha.html

[T57] Scala：模式匹配
来源：http://hz.dashuyun.cn/gtdsdmtgvy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.redwolf501.top/gtbtipjzsn.html

[T58] Scala：函数定义
来源：http://hz.jqgfzy.top/gtpbacpbhm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ppjwa.cn/gtawpsjqtk.html

[T59] Scala：循环
来源：http://hz.vqdsnc.cn/gtugmjjxja.html

for (i <- 1 to 10) println(i)
来源：http://hz.shzxlz.cn/gtmvykheaa.html

[T60] Scala：折叠
来源：http://hz.chenzaomai.com/gtxjqqghwd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jyoumei.cn/gtwicoammt.html

================================================================================
来源：http://hz.redwolf501.top/gthjflnilq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jlsjyb.cn/gtyoclyscj.html

================================================================================
来源：http://hz.fengsongda.top/gtuoxwlxoo.html

[U01] Py：创建虚拟环境
来源：http://hz.xinyue.icu/gtsedlgmcr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sweek.top/gtyolmgjik.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinqigufen.top/gtxnbezlvn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.316326.xyz/gthxzauqga.html

[U03] Py：加载 .env 配置
来源：http://hz.shuidangran.top/gtuhduusne.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gaohongyu789.top/gtrzelqtfn.html

[U04] Py：变量调试打印
来源：http://hz.tanke756.top/gtjbtnchee.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinghuilouyu.cn/gtivtukdhg.html

[U05] Py：列表去重且保序
来源：http://hz.yuanzhike.top/gtsmxofzfg.html

list(dict.fromkeys(arr))
来源：http://hz.daxiang520.top/gtyulkhrbe.html

[U06] Py：合并两个字典
来源：http://hz.xuanzx.com/gtigqavbau.html

{**a, **b}
来源：http://hz.ywan-chungtsiang.top/gtdqfwynvq.html

[U07] Py：反转字典键值
来源：http://hz.zhoulong.xyz/gtphmjkkpr.html

{v: k for k, v in d.items()}
来源：http://hz.cucudq.cn/gtngrqpffx.html

[U08] Py：展平二维列表
来源：http://hz.dashuyun.cn/gtosmrmyny.html

[y for x in nested for y in x]
来源：http://hz.jinyuanbaomall.cn/gtlwkeusbc.html

[U09] Py：字典取最大值的键
来源：http://hz.meibo888.top/gtexlwikhc.html

max(d, key=d.get)
来源：http://hz.aibaodan.cn/gtricaumkp.html

[U10] Py：按值排序字典
来源：http://hz.zhiwuduotai.top/gtjwydhcxp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gaohongyu789.top/gtcksysoro.html

[U11] Py：生成器表达式
来源：http://hz.bjfxy.top/gtxdgmbdje.html

(x * 2 for x in arr)
来源：http://hz.yj20258.top/gtwiiuywrm.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.haohaochexian.top/gtemzcyvpo.html

Counter(arr).most_common(3)
来源：http://hz.smart0.xyz/gtiodnxjvc.html

[U13] Py：固定长度队列
来源：http://hz.gogol.net.cn/gtbsdkxcgq.html

deque(maxlen=10)
来源：http://hz.9152youxi.cn/gtvujpsomj.html

[U14] Py：分组收集到列表
来源：http://hz.ppjwa.cn/gtggoibsyd.html

defaultdict(list)
来源：http://hz.iojbl.cn/gtejcxqkig.html

[U15] Py：高精度计时
来源：http://hz.yj202588.top/gtnkpmwqvw.html

t = time.perf_counter()
来源：http://hz.yj20258.top/gtsirkoune.html

[U16] Py：命令行参数解析
来源：http://hz.nanxinkj.top/gtydkjubym.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.tian-w.cn/gtrawbsxuq.html

[U17] Py：初始化日志
来源：http://hz.havefunace.top/gtdjghisyu.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hysaishi.cn/gtwryalavh.html

[U18] Py：预编译正则
来源：http://hz.shanyushiyangtech.top/gtrwrheohm.html

pat = re.compile(r"\d+")
来源：http://hz.gogol.net.cn/gtpnlscrii.html

[U19] Py：正则替换带回调
来源：http://hz.shanyushiyangtech.top/gtdkvjggxc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhijiandao.cn/gtznixwywm.html

[U20] Py：缓存函数结果
来源：http://hz.chenzaomai.com/gtigabxmhn.html

@functools.lru_cache(maxsize=None)
来源：http://hz.bjfxy.top/gtejnilkfk.html

[U21] Py：自定义上下文管理器
来源：http://hz.tanke756.top/gtfzvkcnzs.html

@contextlib.contextmanager
来源：http://hz.daria6918.cn/gtabunxlqm.html

[U22] Py：矩阵转置
来源：http://hz.zhengqikj.top/gtalcadknm.html

list(zip(*m))
来源：http://hz.yj202588.top/gtopyfwdgq.html

[U23] Py：分块读取大文件
来源：http://hz.quarkkingdee.top/gtvrditybv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.316326.xyz/gtsntvxyoo.html

[U24] Py：路径操作
来源：http://hz.daria6918.cn/gtxqreffnr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhoulong.xyz/gtlaccpsgv.html

[U25] Py：CSV 按字典读
来源：http://hz.cucudq.cn/gtqrbvjxdi.html

csv.DictReader(f)
来源：http://hz.jqgufenzy.top/gtectaedyh.html

[U26] Py：并发下载
来源：http://hz.ehwqpu.com/gtkedelsdc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jiagoushi.top/gtltrcgpie.html

[U27] Py：异步 HTTP
来源：http://hz.ehwqpu.com/gttdcvxxhv.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.pycfn.com/gtrlpfdohh.html

[U28] Py：类型别名
来源：http://hz.cucudq.cn/gtjstbccug.html

UserId = int
来源：http://hz.mhx1999.top/gtogaxlzhm.html

[U29] Py：属性校验
来源：http://hz.ivvv.top/gtcxxfbzmh.html

@property 与 @x.setter 配合
来源：http://hz.jiagoushi.top/gtbkmeteha.html

[U30] Py：数据类
来源：http://hz.hywenlv.cn/gtmihosalh.html

@dataclass(slots=True)
来源：http://hz.hfpthk.cn/gtlcvaupue.html

[U31] Py：单测
来源：http://hz.yvedp.cn/gtkxkosxgl.html

python -m pytest -q
来源：http://hz.yvedp.cn/gttohbluae.html

[U32] Py：代码格式化
来源：http://hz.dashuyun.cn/gtsagcytpm.html

ruff format . && ruff check --fix .
来源：http://hz.zhongyouzk.top/gtmujtrxnq.html

[U33] Py：打包发布
来源：http://hz.mhx1999.top/gtgbjzuehl.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shzxlz.cn/gtdbnenarm.html

[U34] Py：判断编码
来源：http://hz.0kj1m.cn/gtpsfknttd.html

chardet.detect(raw)
来源：http://hz.sufxvd.cn/gtynmdkawb.html

[U35] Py：发送邮件
来源：http://hz.hongshengwenyu.top/gtuadpsqhl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.kuanghao11.cn/gtumavzsix.html

[U36] Py：定时任务
来源：http://hz.shzxlz.cn/gthpazostj.html

schedule.every(10).minutes.do(job)
来源：http://hz.xuetiantiany.cn/gtqfqcizrx.html

[U37] Py：读写 Excel
来源：http://hz.yj20258.top/gtvedacxzl.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.dianchejie.cn/gtwgwlkxov.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhixingplan.top/gtbztqiahb.html

Path(__file__).resolve().parent
来源：http://hz.yongpay.top/gtkgorkdop.html

[U39] Py：判断是否在交互环境
来源：http://hz.shuidangran.top/gtxnpcumyw.html

sys.stdout.isatty()
来源：http://hz.jianghu66.top/gtaugjabft.html

[U40] Py：打印到标准错误
来源：http://hz.yvedp.cn/gtvvhfbavd.html

print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtdjcharlw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhixingplan.top/gtsakclfnh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.havefunace.top/gtbjdyytxf.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sufxvd.cn/gtobhiehxg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.9152youxi.cn/gthjwwsxzl.html

[U43] PHP：声明命名空间
来源：http://hz.ivvv.top/gtjvahvoct.html

namespace App\Http;
来源：http://hz.c1oappe.top/gtnitquyzk.html

[U44] PHP：开启严格类型
来源：http://hz.smart0.xyz/gtjrbhsfdl.html

declare(strict_types=1);
来源：http://hz.cucudq.cn/gttfydeguf.html

[U45] PHP：类型声明与返回类型
来源：http://hz.nanxinkj.top/gtgbiyxiax.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtyyjohopr.html

[U46] PHP：可空类型
来源：http://hz.wangshuangyany.cn/gtpzncgzco.html

?string $name = null
来源：http://hz.quarkkingdee.top/gtxldfuurk.html

[U47] PHP：联合类型
来源：http://hz.hongshengwenyu.top/gtlurmzlee.html

int|string $id
来源：http://hz.gaohongyu789.top/gttplhoaks.html

[U48] PHP：纯枚举
来源：http://hz.jqgufenzy.top/gtxztqrfhr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jiagoushi.top/gtzidtdxvp.html

[U49] PHP：只读属性
来源：http://hz.yangfankeji.com/gtlvnydtdh.html

public readonly string $name
来源：http://hz.yj20258888.top/gtpuymhsar.html

[U50] PHP：构造器属性提升
来源：http://hz.kuanghao11.cn/gtzgiqyjvr.html

public function __construct(private int $id) {}
来源：http://hz.yongpay.top/gtxcpovufm.html

[U51] PHP：数组解构
来源：http://hz.ydzc1.top/gtrhqdtkcs.html

[$a, $b] = $arr;
来源：http://hz.yonumen.top/gtovvrcena.html

[U52] PHP：箭头函数
来源：http://hz.kuanghao11.cn/gtgckkpnpx.html

$double = fn($x) => $x * 2;
来源：http://hz.quarkkingdee.top/gtnrvxqkdp.html

[U53] PHP：空合并运算符
来源：http://hz.316326.xyz/gtowgbwhuh.html

$v = $a ?? $b ?? "default";
来源：http://hz.aibaodan.cn/gtlaamqvtj.html

[U54] PHP：空安全调用
来源：http://hz.zdqjudy.top/gtrfgfitty.html

$obj?->method()
来源：http://hz.nwbrower.top/gtnohvuhos.html

[U55] PHP：match 表达式
来源：http://hz.pycfn.com/gtbqoskkep.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.chenlongwang.top/gtlerxugfp.html

[U56] PHP：命名参数
来源：http://hz.xingfuxueyuan.xyz/gtsgamwbic.html

f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtbibcletq.html

[U57] PHP：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtobrbydub.html

"值: {$a}"
来源：http://hz.andypj.xyz/gthrkmqogn.html

[U58] PHP：数组三件套
来源：http://hz.yj20258.top/gtyuntrqlq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jqgfzy.top/gtildvfslr.html

[U59] PHP：自定义排序
来源：http://hz.cqqwz.cn/gtijyygdjl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.9152youxi.cn/gtuacpmheq.html

[U60] PHP：JSON 编解码
来源：http://hz.chenzaomai.com/gtnvzwxcjn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.andypj.xyz/gtohwbynfi.html

[U61] PHP：正则
来源：http://hz.xingfuxueyuan.xyz/gtzexyjymg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangtech.top/gtpdyovpdw.html

[U62] PHP：日期对象
来源：http://hz.smart0.xyz/gtckxgsjdb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sysykeji.top/gtnadisqrj.html

[U63] PHP：文件读写
来源：http://hz.shanyushiyangtech.top/gtmsjrczvx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cdnleiting.top/gtgjfotdzt.html

[U64] PHP：目录遍历
来源：http://hz.nanxuanxn.top/gtpbvcfpdx.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sysykeji.top/gtsbpnrkhm.html

[U65] PHP：会话
来源：http://hz.shanyushiyangtech.top/gtlcjocsaa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jinqigfzy.top/gtuipycosl.html

[U66] PHP：设置 Cookie
来源：http://hz.gaohongyu789.top/gtlednekfn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.chenjidiqi.icu/gtpkgkcfgj.html

[U67] PHP：处理文件上传
来源：http://hz.xinyue.icu/gtrqeihspj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhoulong.xyz/gtnmsbrfzp.html

[U68] PHP：PDO 连接
来源：http://hz.fzhhl.top/gtxqrgfete.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hnqzz.top/gtsekhsxxo.html

[U69] PHP：PDO 预处理
来源：http://hz.ivvv.top/gtsvjtgipj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zdqjudy.top/gtnvatjwzg.html

[U70] PHP：PDO 事务
来源：http://hz.xingfuxueyuan.xyz/gtjkssrryi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shanyushiyangkeji.top/gtrotsoten.html

[U71] PHP：抛出异常
来源：http://hz.havefunace.top/gtbjsitkov.html

throw new RuntimeException("失败", 500);
来源：http://hz.ehwqpu.com/gtwqcmmrdi.html

[U72] PHP：写错误日志
来源：http://hz.jinyuanbaomall.cn/gttvtodtkw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yanxiufei.cn/gtbfssgpnk.html

[U73] PHP：读取 ini 配置
来源：http://hz.ehwqpu.com/gtjuocjhvq.html

parse_ini_file("config.ini", true)
来源：http://hz.jinqigfzy.top/gtxenigpkq.html

[U74] PHP：读取环境变量
来源：http://hz.ydzc1.top/gtimwsjmmb.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gaohongyu789.top/gtzfdnvvsy.html

[U75] PHP：依赖注入
来源：http://hz.xylfe.cn/gtcquqzrte.html

composer require psr/container
来源：http://hz.yuanzhike.top/gtmwwhicdd.html

[U76] PHP：简单路由
来源：http://hz.xuetiantiany.cn/gtizsbrgre.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.gaohongyu789.top/gtctszluob.html

[U77] PHP：模板渲染
来源：http://hz.shangyingyoupin.top/gtvldveozp.html

composer require twig/twig
来源：http://hz.yueranfly.top/gtlpdkmqad.html

[U78] PHP：单元测试
来源：http://hz.havefunace.top/gtunpquvgh.html

composer require --dev phpunit/phpunit
来源：http://hz.mhx1999.top/gtcujogfqp.html


<!-- 参考信息 -->