代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shangyingyoupin.top/gtefmlzngo.html

[S55] C++：结构化绑定
来源：http://hz.iojbl.cn/gtckwjxgxe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgfzy.top/gtxcjoyljb.html

[S56] C++：optional
来源：http://hz.yvedp.cn/gtusqdadkg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ydzc1.top/gtdnnuelin.html

[S57] C++：编译期常量
来源：http://hz.zhoulong.xyz/gtjikeowjh.html

constexpr int N = 10;
来源：http://hz.aizwys.cn/gtqziarzto.html

[S58] C++：命名空间
来源：http://hz.52xcode.cn/gtwfrmlusc.html

namespace ns { int f() { return 1; } }
来源：http://hz.jiagoushi.top/gtggsshwhx.html

[S59] C++：静态断言
来源：http://hz.tian-w.cn/gtkfsrvlqo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.meibo888.top/gtqybtfzos.html

[S60] C++：遍历并删除元素
来源：http://hz.hnxiangtu.top/gtzrjytizz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj202588.top/gttvnwvouq.html

================================================================================
来源：http://hz.andypj.xyz/gtrfcuwvrm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tianlin.xyz/gthntplehz.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtgazowkbr.html

[T01] Kotlin：Hello World
来源：http://hz.gaohongyu789.top/gtyrneclmd.html

println("Hello")
来源：http://hz.jiagoushi.top/gtzwnnksnr.html

[T02] Kotlin：变量
来源：http://hz.zhixingplan.top/gtmnivmbds.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.52xcode.cn/gtdcpzoylf.html

[T03] Kotlin：字符串模板
来源：http://hz.xuanzx.com/gtodogosts.html

"值: $b"
来源：http://hz.haohaochexian.top/gtdkpjiuti.html

[T04] Kotlin：空安全
来源：http://hz.yj20258.top/gtmdyjhdeq.html

val n: String? = null;  n?.length
来源：http://hz.shangyingyoupin.top/gtipqojusb.html

[T05] Kotlin：when 表达式
来源：http://hz.52xcode.cn/gtxgdvtnnv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.kuanghao11.cn/gtizpgaydi.html

[T06] Kotlin：集合映射
来源：http://hz.yuxming.cn/gtbtwtdolm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnqzz.top/gtjcsmlnyk.html

[T07] Kotlin：集合过滤
来源：http://hz.guowangkeji.top/gttktlfxhm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.wangdashe.top/gtwsgtoxuw.html

[T08] Kotlin：数据类
来源：http://hz.svipenyu.cn/gttijcdeqw.html

data class User(val name: String, val age: Int)
来源：http://hz.hnqzz.top/gtdlpsjtty.html

[T09] Kotlin：扩展函数
来源：http://hz.sysykeji.top/gtgiitjfdr.html

fun String.exclaim() = this + "!"
来源：http://hz.hammf.cn/gtogstreel.html

[T10] Kotlin：默认参数
来源：http://hz.hammf.cn/gteqjienht.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xuanzx.com/gttsqkmslx.html

[T11] Kotlin：协程
来源：http://hz.jinqigfzy.top/gtfodupkht.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.haohaochexian.top/gtqwazdvhv.html

[T12] Kotlin：解构声明
来源：http://hz.mhx1999.top/gtczuiithw.html

val (a, b) = Pair(1, 2)
来源：http://hz.jinyuanbaomall.cn/gtngnaeitw.html

[T13] Kotlin：只读 Map
来源：http://hz.daria6918.cn/gtphjiknfl.html

val m = mapOf("a" to 1)
来源：http://hz.aibaodan.cn/gtrzgrkyds.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gtngccvskf.html

for (i in 1..10) println(i)
来源：http://hz.ivvv.top/gttumlyinb.html

[T15] Kotlin：接口
来源：http://hz.kuanghao11.cn/gtfoczhdpg.html

interface Shape { fun area(): Double }
来源：http://hz.yanxiufei.cn/gtijpudwtn.html

[T16] Swift：Hello World
来源：http://hz.jianghu66.top/gtseuoabae.html

print("Hello")
来源：http://hz.pycfn.com/gtbhgwsbii.html

[T17] Swift：变量与常量
来源：http://hz.ppjwa.cn/gtcqklgaxr.html

var a = 1;  let b = 2
来源：http://hz.bjfxy.top/gtmuxbrxis.html

[T18] Swift：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtmqafdjkz.html

"值: \(b)"
来源：http://hz.jinqigufen.top/gtdpmksmzz.html

[T19] Swift：可选绑定
来源：http://hz.nanxinkj.top/gtqkdnsdao.html

if let n = opt { print(n) }
来源：http://hz.redwolf501.top/gtjydgkzup.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtioqzjgvy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.bjfxy.top/gttreuotez.html

[T21] Swift：遍历
来源：http://hz.yuanzhike.top/gtpfixavjr.html

for x in a { print(x) }
来源：http://hz.jyoumei.cn/gtkiujpsga.html

[T22] Swift：字典
来源：http://hz.yj202588.top/gtetgpltfh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yuxming.cn/gtjbovjida.html

[T23] Swift：函数
来源：http://hz.yonumen.top/gtxbcdozim.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinyuanbaomall.cn/gtgkhxwqwj.html

[T24] Swift：闭包
来源：http://hz.cashguo.top/gtolovbnen.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shuidangran.top/gtqvlksvge.html

[T25] Swift：结构体
来源：http://hz.hnxiangtu.top/gtkysstcfq.html

struct P { var x: Int }
来源：http://hz.xingfuxueyuan.xyz/gtcjhpwhuc.html

[T26] Swift：类与重写
来源：http://hz.ydjk.org.cn/gtwqzamcbd.html

class A: Base { override func f() {} }
来源：http://hz.jqgfzy.top/gtkckjedqc.html

[T27] Swift：错误处理
来源：http://hz.cheryme.top/gtatpoqudb.html

do { try f() } catch { print(error) }
来源：http://hz.yongpay.top/gtovphblhs.html

[T28] Swift：枚举
来源：http://hz.c1oappe.top/gtvinfkeot.html

enum Color { case red, green }
来源：http://hz.havefunace.top/gtrrkuntzc.html

[T29] Swift：guard 提前返回
来源：http://hz.fzhhl.top/gtxrfymyqd.html

guard let x = opt else { return }
来源：http://hz.xylfe.cn/gtlaqckyha.html

[T30] Swift：协议
来源：http://hz.hongshengwenyu.top/gtohkiwkpy.html

protocol Shape { func area() -> Double }
来源：http://hz.ppjwa.cn/gtbywshqcg.html

[T31] Lua：Hello World
来源：http://hz.jinghuilouyu.cn/gtgjrzjacf.html

print("Hello")
来源：http://hz.havefunace.top/gtgydlesmd.html

[T32] Lua：局部变量
来源：http://hz.daria6918.cn/gtdmkwpzbw.html

local a = 1
来源：http://hz.chenzaomai.com/gtjmwlaklb.html

[T33] Lua：表（数组）
来源：http://hz.ydjk.org.cn/gthxnhlkey.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shzxlz.cn/gtkigxdoax.html

[T34] Lua：遍历表
来源：http://hz.ybcxt.top/gtfyespodq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yj20258.top/gtjheuszzf.html

[T35] Lua：字典表
来源：http://hz.xuanzx.com/gtzimgzhfn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cdnleiting.top/gtonalvoer.html

[T36] Lua：函数
来源：http://hz.shuidangran.top/gtkttxcwot.html

function add(a, b) return a + b end
来源：http://hz.shzxlz.cn/gtxaoahdnj.html

[T37] Lua：字符串拼接
来源：http://hz.gaohongyu789.top/gtekofakjp.html

"a" .. "b"
来源：http://hz.tianlin.xyz/gtdlevzkqo.html

[T38] Lua：条件
来源：http://hz.gogol.net.cn/gtoqxmgohm.html

if x > 0 then print("正") end
来源：http://hz.nanxuanxn.top/gtuogwrwdz.html

[T39] Lua：模式匹配
来源：http://hz.nwbrower.top/gtlhbkaqhg.html

string.find(s, "%d+")
来源：http://hz.nanxuanxn.top/gtkdvcdtum.html

[T40] Lua：元表
来源：http://hz.tian-w.cn/gtfupylfyw.html

setmetatable({}, { __index = base })
来源：http://hz.ydzc1.top/gticwgpsmo.html

[T41] Perl：Hello World
来源：http://hz.0kj1m.cn/gtpfnbuwfa.html

print "Hello\n";
来源：http://hz.yj202588.top/gtfzlxrbqf.html

[T42] Perl：变量类型
来源：http://hz.52xcode.cn/gtsvscnfso.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zycfv.cn/gttfdvjetu.html

[T43] Perl：字符串插值
来源：http://hz.wangshuangyany.cn/gtjjbrxdgo.html

"值: $a"
来源：http://hz.yonumen.top/gtbkwrpspu.html

[T44] Perl：条件
来源：http://hz.hammf.cn/gtqczrvpmg.html

if ($a > 0) { print "正"; }
来源：http://hz.xuetiantiany.cn/gtqigjyfel.html

[T45] Perl：数组遍历
来源：http://hz.shzxlz.cn/gtprcmryux.html

for my $x (@arr) { print $x; }
来源：http://hz.redwolf501.top/gtjoajwspw.html

[T46] Perl：哈希操作
来源：http://hz.gzhubu.top/gtfgvyavoq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ydzc1.top/gtrrfzbdac.html

[T47] Perl：正则捕获
来源：http://hz.sufxvd.cn/gtfjakafsj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.bjfxy.top/gtasymtrhp.html

[T48] Perl：正则替换
来源：http://hz.yvedp.cn/gtyqivdqha.html

$s =~ s/old/new/g;
来源：http://hz.yonumen.top/gtnatmngzy.html

[T49] Perl：函数
来源：http://hz.meibo888.top/gttriuovan.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cashguo.top/gthxbcaqgf.html

[T50] Perl：逐行读文件
来源：http://hz.zhoulong.xyz/gtjuqkyeqv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.daria6918.cn/gtrbhcxikc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.smart0.xyz/gtlfzxuypa.html

[T51] Scala：Hello World
来源：http://hz.shanyushiyangkeji.top/gtpxutyakm.html

println("Hello")
来源：http://hz.ydjk.org.cn/gtrqryfgab.html

[T52] Scala：变量
来源：http://hz.hammf.cn/gtmrdotltk.html

val a = 1;  var b = 2
来源：http://hz.havefunace.top/gttazkigdi.html

[T53] Scala：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtawcgbwoc.html

s"值: $b"
来源：http://hz.nanxinkj.top/gtivnrqyri.html

[T54] Scala：集合映射
来源：http://hz.chenzaomai.com/gtkougbvlw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.tian-w.cn/gtjbkcktdi.html

[T55] Scala：集合过滤
来源：http://hz.sxryk.cn/gtefwigcbr.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.snrcjt.cn/gtgoacvizl.html

[T56] Scala：样例类
来源：http://hz.hfpthk.cn/gtrlzfovfq.html

case class User(name: String, age: Int)
来源：http://hz.jinqigufen.top/gtyhfikhfe.html

[T57] Scala：模式匹配
来源：http://hz.feifeiyinyue.top/gthdebgaby.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.c1oappe.top/gtumokdhbm.html

[T58] Scala：函数定义
来源：http://hz.hnqzz.top/gthgxovtjy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hongshengwenyu.top/gtmcchxapp.html

[T59] Scala：循环
来源：http://hz.yonumen.top/gthukevblp.html

for (i <- 1 to 10) println(i)
来源：http://hz.jyoumei.cn/gtyiaypnry.html

[T60] Scala：折叠
来源：http://hz.cucudq.cn/gtxxxalflb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.snrcjt.cn/gtgjkbrspb.html

================================================================================
来源：http://hz.havefunace.top/gtuwjihppf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhengqikj.top/gtlghogtap.html

================================================================================
来源：http://hz.andypj.xyz/gtzqxmrsbv.html

[U01] Py：创建虚拟环境
来源：http://hz.nanxuanxn.top/gtnsouadel.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cashguo.top/gthcbqikqy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cdnleiting.top/gtujlgwutb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinyuanbaomall.cn/gtjnhmedfp.html

[U03] Py：加载 .env 配置
来源：http://hz.gogol.net.cn/gtwfbnrkbl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhongyouzk.top/gtbhbgeijy.html

[U04] Py：变量调试打印
来源：http://hz.svipenyu.cn/gttckpgkxf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.chenzaomai.com/gttiqwylty.html

[U05] Py：列表去重且保序
来源：http://hz.shuidangran.top/gturtqylvr.html

list(dict.fromkeys(arr))
来源：http://hz.zhixingplan.top/gthixflyrt.html

[U06] Py：合并两个字典
来源：http://hz.sxryk.cn/gtbvuhiwlv.html

{**a, **b}
来源：http://hz.52xcode.cn/gtibfblbtt.html

[U07] Py：反转字典键值
来源：http://hz.smart0.xyz/gtauxgylrk.html

{v: k for k, v in d.items()}
来源：http://hz.nanxinkj.top/gtbiugalnq.html

[U08] Py：展平二维列表
来源：http://hz.jiagoushi.top/gtluyucxcz.html

[y for x in nested for y in x]
来源：http://hz.shzxlz.cn/gtscfgxepo.html

[U09] Py：字典取最大值的键
来源：http://hz.jinghuilouyu.cn/gthqzpqwrf.html

max(d, key=d.get)
来源：http://hz.sysykeji.top/gtrpsgdmoi.html

[U10] Py：按值排序字典
来源：http://hz.fzhhl.top/gthrlmwute.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.9152youxi.cn/gtgwpfezpx.html

[U11] Py：生成器表达式
来源：http://hz.cashguo.top/gtuystxktq.html

(x * 2 for x in arr)
来源：http://hz.hysaishi.cn/gtdpajlwjm.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cheryme.top/gthmzimggq.html

Counter(arr).most_common(3)
来源：http://hz.jianghu66.top/gtravhtbfo.html

[U13] Py：固定长度队列
来源：http://hz.zhaomingkeji.xyz/gtyborzmpv.html

deque(maxlen=10)
来源：http://hz.ppjwa.cn/gtkpsfyovv.html

[U14] Py：分组收集到列表
来源：http://hz.kuanghao11.cn/gtnpftzjam.html

defaultdict(list)
来源：http://hz.feifeiyinyue.top/gtsocfkrcj.html

[U15] Py：高精度计时
来源：http://hz.xuetiantiany.cn/gtjrndacnj.html

t = time.perf_counter()
来源：http://hz.dashuyun.cn/gthupodeli.html

[U16] Py：命令行参数解析
来源：http://hz.yj20258.top/gtlmktohrz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.meibo888.top/gtfgzdjokt.html

[U17] Py：初始化日志
来源：http://hz.nanxuanxn.top/gtzaapzhxp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yuanzhike.top/gtzpcovmyy.html

[U18] Py：预编译正则
来源：http://hz.jinyuanbaomall.cn/gtdatkqsts.html

pat = re.compile(r"\d+")
来源：http://hz.mhx1999.top/gttxyvzeoo.html

[U19] Py：正则替换带回调
来源：http://hz.chenzaomai.com/gtsfovvtph.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.haohaochexian.top/gtsdcunspv.html

[U20] Py：缓存函数结果
来源：http://hz.xinyue.icu/gtwyzhnmvw.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xuanzx.com/gtattuaqwj.html

[U21] Py：自定义上下文管理器
来源：http://hz.0kj1m.cn/gteowczmus.html

@contextlib.contextmanager
来源：http://hz.haohaochexian.top/gtgihwmyuq.html

[U22] Py：矩阵转置
来源：http://hz.jianghu66.top/gtvgzlacgv.html

list(zip(*m))
来源：http://hz.9152youxi.cn/gtyzcqpvar.html

[U23] Py：分块读取大文件
来源：http://hz.tanke756.top/gtbbxdxpns.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.kuanghao11.cn/gtpvyextll.html

[U24] Py：路径操作
来源：http://hz.dianchejie.cn/gtyegjkigx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.havefunace.top/gtoirqndeu.html

[U25] Py：CSV 按字典读
来源：http://hz.cucudq.cn/gtevkcvrld.html

csv.DictReader(f)
来源：http://hz.yuxming.cn/gtvdxtsiwo.html

[U26] Py：并发下载
来源：http://hz.xziqi.cn/gtqjwaqctq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sweek.top/gtpbcvrhdp.html

[U27] Py：异步 HTTP
来源：http://hz.svipenyu.cn/gtmmvvpzie.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xingfuxueyuan.xyz/gtlgrnyzof.html

[U28] Py：类型别名
来源：http://hz.svipenyu.cn/gthvvrempy.html

UserId = int
来源：http://hz.ywan-chungtsiang.top/gtsfknshfi.html

[U29] Py：属性校验
来源：http://hz.aibaodan.cn/gtvrjwqgji.html

@property 与 @x.setter 配合
来源：http://hz.dianchejie.cn/gtwnrhxhlr.html

[U30] Py：数据类
来源：http://hz.nanxinkj.top/gtykwnfgjd.html

@dataclass(slots=True)
来源：http://hz.zhijiandao.cn/gtnznhxner.html

[U31] Py：单测
来源：http://hz.bjfxy.top/gtuqgdxqpf.html

python -m pytest -q
来源：http://hz.ivvv.top/gtnkojumvn.html

[U32] Py：代码格式化
来源：http://hz.jinqigufen.top/gtkvokjfwl.html

ruff format . && ruff check --fix .
来源：http://hz.pycfn.com/gtesnkllyf.html

[U33] Py：打包发布
来源：http://hz.ybcxt.top/gtrhsyaiqv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jyoumei.cn/gtsdgoxmvd.html

[U34] Py：判断编码
来源：http://hz.feifeiyinyue.top/gttxfwgbpm.html

chardet.detect(raw)
来源：http://hz.pycfn.com/gtyeqlhvfc.html

[U35] Py：发送邮件
来源：http://hz.yj20258.top/gtaeabltur.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhiwuduotai.top/gtvduknfuo.html

[U36] Py：定时任务
来源：http://hz.yvedp.cn/gtjzwhaxuo.html

schedule.every(10).minutes.do(job)
来源：http://hz.svipenyu.cn/gtjrjbomyj.html

[U37] Py：读写 Excel
来源：http://hz.yj20258.top/gthypcrowd.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.daxiang520.top/gtjunxriec.html

[U38] Py：获取脚本所在目录
来源：http://hz.smart0.xyz/gtuqzttkvo.html

Path(__file__).resolve().parent
来源：http://hz.shuidangran.top/gtipvldoww.html

[U39] Py：判断是否在交互环境
来源：http://hz.wangdashe.top/gthsnmknpc.html

sys.stdout.isatty()
来源：http://hz.dashuyun.cn/gtdrctbnfe.html

[U40] Py：打印到标准错误
来源：http://hz.ppjwa.cn/gtjnvddmqs.html

print("err", file=sys.stderr)
来源：http://hz.aibaodan.cn/gtivhbqlia.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.feifeiyinyue.top/gtapzqphml.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sxryk.cn/gtsfrdlrea.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.aibaodan.cn/gtxghsrrpf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.dianchejie.cn/gtgtgxhfxx.html

[U43] PHP：声明命名空间
来源：http://hz.tanke756.top/gtiitpeyqz.html

namespace App\Http;
来源：http://hz.wangdashe.top/gtxzbknhhf.html

[U44] PHP：开启严格类型
来源：http://hz.cdnleiting.top/gtfsxsceou.html

declare(strict_types=1);
来源：http://hz.redwolf501.top/gtjteuqmcv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.tanke756.top/gtaxlfryrt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtbohpeuga.html

[U46] PHP：可空类型
来源：http://hz.feifeiyinyue.top/gtavefqnxh.html

?string $name = null
来源：http://hz.xuetiantiany.cn/gtudkbejvx.html

[U47] PHP：联合类型
来源：http://hz.dianchejie.cn/gtfzcsppbi.html

int|string $id
来源：http://hz.yvedp.cn/gtuhjaafhs.html

[U48] PHP：纯枚举
来源：http://hz.feifeiyinyue.top/gtvuyotoin.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.sufxvd.cn/gtqgcntdmt.html

[U49] PHP：只读属性
来源：http://hz.shangyingyoupin.top/gtdhgcwumv.html

public readonly string $name
来源：http://hz.sxryk.cn/gtxfvnrvmk.html

[U50] PHP：构造器属性提升
来源：http://hz.bjfxy.top/gtoqvrfeem.html

public function __construct(private int $id) {}
来源：http://hz.iojbl.cn/gtnahediuq.html

[U51] PHP：数组解构
来源：http://hz.chenjidiqi.icu/gtpifvieso.html

[$a, $b] = $arr;
来源：http://hz.fengsongda.top/gtncnbpllw.html

[U52] PHP：箭头函数
来源：http://hz.dashuyun.cn/gtnwpcglgg.html

$double = fn($x) => $x * 2;
来源：http://hz.tianlin.xyz/gtoyslcobo.html

[U53] PHP：空合并运算符
来源：http://hz.jiagoushi.top/gthgsmxsoq.html

$v = $a ?? $b ?? "default";
来源：http://hz.hnxiangtu.top/gtotqykwiu.html

[U54] PHP：空安全调用
来源：http://hz.cashguo.top/gtrxedpixi.html

$obj?->method()
来源：http://hz.tanke756.top/gtvwhzqmic.html

[U55] PHP：match 表达式
来源：http://hz.c1oappe.top/gtjhzbfswu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xinyue.icu/gtygqqwgff.html

[U56] PHP：命名参数
来源：http://hz.52xcode.cn/gtlshxisxm.html

f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gteaqwpuxg.html

[U57] PHP：字符串插值
来源：http://hz.iojbl.cn/gtgffmsbib.html

"值: {$a}"
来源：http://hz.shangyingyoupin.top/gtfcewnbyr.html

[U58] PHP：数组三件套
来源：http://hz.haohaochexian.top/gtggmkiews.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yj20258.top/gtddwswnmi.html

[U59] PHP：自定义排序
来源：http://hz.gotoacloud.top/gtzwwiswrn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sysykeji.top/gtnnvtlxkb.html

[U60] PHP：JSON 编解码
来源：http://hz.yuxming.cn/gtlgsjdeaj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.chenjidiqi.icu/gtpowcoyep.html

[U61] PHP：正则
来源：http://hz.pycfn.com/gtaexwlcti.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yangfankeji.com/gtsqktmtug.html

[U62] PHP：日期对象
来源：http://hz.nanxuanxn.top/gtjelsdqkg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.guowangkeji.top/gtxgwlqopn.html

[U63] PHP：文件读写
来源：http://hz.cashguo.top/gtidbyglcb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.meibo888.top/gtewbpqluo.html

[U64] PHP：目录遍历
来源：http://hz.svipenyu.cn/gtiuramfaq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.dashuyun.cn/gtxqdkqqug.html

[U65] PHP：会话
来源：http://hz.yvedp.cn/gtkxmyqobz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.birdmap.top/gtivefdtos.html

[U66] PHP：设置 Cookie
来源：http://hz.redwolf501.top/gtkvdwotet.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.iojbl.cn/gtjbvbekud.html

[U67] PHP：处理文件上传
来源：http://hz.aibaodan.cn/gtasgryoym.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.aizwys.cn/gtyadrzhzr.html

[U68] PHP：PDO 连接
来源：http://hz.svipenyu.cn/gtiwlwmsgo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhijiandao.cn/gtugfqwvmo.html

[U69] PHP：PDO 预处理
来源：http://hz.chenlongwang.top/gttllsmkkm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ppjwa.cn/gtwlcmufal.html

[U70] PHP：PDO 事务
来源：http://hz.birdmap.top/gtptidjzcu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hysaishi.cn/gtmtqnridh.html

[U71] PHP：抛出异常
来源：http://hz.tanke756.top/gtgydybmky.html

throw new RuntimeException("失败", 500);
来源：http://hz.jqgufenzy.top/gtekxwsfop.html

[U72] PHP：写错误日志
来源：http://hz.xinyue.icu/gtszzshyog.html

error_log("失败: " . $e->getMessage());
来源：http://hz.sxryk.cn/gtastlxmun.html

[U73] PHP：读取 ini 配置
来源：http://hz.yj202588.top/gtnocwbmmm.html

parse_ini_file("config.ini", true)
来源：http://hz.svipenyu.cn/gteoqorhxw.html

[U74] PHP：读取环境变量
来源：http://hz.snrcjt.cn/gtivrqsqfc.html

getenv("APP_ENV") ?: "production"
来源：http://hz.mhx1999.top/gtyqpzuwju.html

[U75] PHP：依赖注入
来源：http://hz.shuidangran.top/gtryppxfnk.html

composer require psr/container
来源：http://hz.xingfuxueyuan.xyz/gtcofzxedb.html

[U76] PHP：简单路由
来源：http://hz.guannengcc.top/gtgiiafhhz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ehwqpu.com/gtngrjdjnl.html

[U77] PHP：模板渲染
来源：http://hz.chenlongwang.top/gtafeszdgc.html

composer require twig/twig
来源：http://hz.chenlongwang.top/gtdeyxbcgq.html

[U78] PHP：单元测试
来源：http://hz.meibo888.top/gtbpvgutyt.html

composer require --dev phpunit/phpunit
来源：http://hz.xylfe.cn/gtyqnvgzse.html

[U79] PHP：静态分析
来源：http://hz.ivvv.top/gtavzfoxrh.html

composer require --dev phpstan/phpstan
来源：http://hz.shzxlz.cn/gtljsgmwma.html

[U80] PHP：代码规范修复
来源：http://hz.yangfankeji.com/gtogehvzjz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zdqjudy.top/gtnnsqcwmk.html


<!-- 参考信息 -->