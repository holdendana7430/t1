代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://hz.316326.xyz/gtkngydvrp.html

[S59] C++：静态断言
来源：http://hz.hywenlv.cn/gtdlqxsbew.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxinkj.top/gtnoypuubs.html

[S60] C++：遍历并删除元素
来源：http://hz.shuidangran.top/gtkqijqcgl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dianchejie.cn/gtyjmoxjet.html

================================================================================
来源：http://hz.316326.xyz/gtdajvaktk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tian-w.cn/gtcorftlhr.html

================================================================================
来源：http://hz.yanxiufei.cn/gtekabpnhb.html

[T01] Kotlin：Hello World
来源：http://hz.shangyingyoupin.top/gteyjtwyrm.html

println("Hello")
来源：http://hz.shzxlz.cn/gtsbofmxke.html

[T02] Kotlin：变量
来源：http://hz.jinyuanbaomall.cn/gtzilsmnkv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangkeji.top/gtdskmvaed.html

[T03] Kotlin：字符串模板
来源：http://hz.sweek.top/gtselzacye.html

"值: $b"
来源：http://hz.jlsjyb.cn/gtsrlkeytx.html

[T04] Kotlin：空安全
来源：http://hz.hnqzz.top/gtgjiqewao.html

val n: String? = null;  n?.length
来源：http://hz.snrcjt.cn/gtkjhfzrju.html

[T05] Kotlin：when 表达式
来源：http://hz.gzhubu.top/gttjuqpwce.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgfzy.top/gtieaeemxk.html

[T06] Kotlin：集合映射
来源：http://hz.shanyushiyangkeji.top/gtjsivwblg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.daxiang520.top/gtaqkswobv.html

[T07] Kotlin：集合过滤
来源：http://hz.vqdsnc.cn/gtfpcnldef.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinyuanbaomall.cn/gtfkregavy.html

[T08] Kotlin：数据类
来源：http://hz.yanxiufei.cn/gtkrmlphek.html

data class User(val name: String, val age: Int)
来源：http://hz.9152youxi.cn/gtiejxsjxt.html

[T09] Kotlin：扩展函数
来源：http://hz.kuanghao11.cn/gtyuhbamdh.html

fun String.exclaim() = this + "!"
来源：http://hz.shangyingyoupin.top/gtufvhyvou.html

[T10] Kotlin：默认参数
来源：http://hz.ehwqpu.com/gtqglmhlfl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhiwuduotai.top/gtzkvhlmwq.html

[T11] Kotlin：协程
来源：http://hz.tian-w.cn/gtdpklytst.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.snrcjt.cn/gtadqjeodr.html

[T12] Kotlin：解构声明
来源：http://hz.tian-w.cn/gtcebtemyi.html

val (a, b) = Pair(1, 2)
来源：http://hz.wangshuangyany.cn/gtxraxrier.html

[T13] Kotlin：只读 Map
来源：http://hz.aibaodan.cn/gtlofzvcbs.html

val m = mapOf("a" to 1)
来源：http://hz.zhijiandao.cn/gtdxiqarym.html

[T14] Kotlin：循环
来源：http://hz.quarkkingdee.top/gtpddlavmo.html

for (i in 1..10) println(i)
来源：http://hz.chenjidiqi.icu/gtihzmcaio.html

[T15] Kotlin：接口
来源：http://hz.ivvv.top/gtykkqwytl.html

interface Shape { fun area(): Double }
来源：http://hz.meibo888.top/gtzbdicstf.html

[T16] Swift：Hello World
来源：http://hz.aibaodan.cn/gtfmcdioui.html

print("Hello")
来源：http://hz.hysaishi.cn/gtggxtbmgq.html

[T17] Swift：变量与常量
来源：http://hz.gogol.net.cn/gtlauiqabe.html

var a = 1;  let b = 2
来源：http://hz.fengsongda.top/gtdbfkoode.html

[T18] Swift：字符串插值
来源：http://hz.tanke756.top/gtaiedngzt.html

"值: \(b)"
来源：http://hz.9152youxi.cn/gtvtwoqqfa.html

[T19] Swift：可选绑定
来源：http://hz.zhengqikj.top/gttejwlpkk.html

if let n = opt { print(n) }
来源：http://hz.fzhhl.top/gtvgcyldvo.html

[T20] Swift：数组操作
来源：http://hz.shuidangran.top/gttzlsywkc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nanxuanxn.top/gtanijlpct.html

[T21] Swift：遍历
来源：http://hz.jqgufenzy.top/gtkizxxdlv.html

for x in a { print(x) }
来源：http://hz.vqdsnc.cn/gtxjzlttex.html

[T22] Swift：字典
来源：http://hz.wangshuangyany.cn/gtaivecrsh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinqigufen.top/gtuvvidsan.html

[T23] Swift：函数
来源：http://hz.svipenyu.cn/gthsbuylgr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ywan-chungtsiang.top/gtvwcckksy.html

[T24] Swift：闭包
来源：http://hz.yangfankeji.com/gtbaadfrfw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.52xcode.cn/gtzaidzdlj.html

[T25] Swift：结构体
来源：http://hz.jqgfzy.top/gtthrxdyep.html

struct P { var x: Int }
来源：http://hz.chenlongwang.top/gttxpphygb.html

[T26] Swift：类与重写
来源：http://hz.xuanzx.com/gtfpzndsju.html

class A: Base { override func f() {} }
来源：http://hz.yongpay.top/gtphjjdkos.html

[T27] Swift：错误处理
来源：http://hz.yj202588.top/gtpxvgqyth.html

do { try f() } catch { print(error) }
来源：http://hz.shangyingyoupin.top/gtvcqtdlia.html

[T28] Swift：枚举
来源：http://hz.hfpthk.cn/gtsptvlsuw.html

enum Color { case red, green }
来源：http://hz.jqgufenzy.top/gtjyohmutl.html

[T29] Swift：guard 提前返回
来源：http://hz.gaohongyu789.top/gtrplepmfp.html

guard let x = opt else { return }
来源：http://hz.smart0.xyz/gtdtxseoxx.html

[T30] Swift：协议
来源：http://hz.andypj.xyz/gtyrpfcflh.html

protocol Shape { func area() -> Double }
来源：http://hz.yanxiufei.cn/gtznngeapl.html

[T31] Lua：Hello World
来源：http://hz.chenjidiqi.icu/gtrqveqezt.html

print("Hello")
来源：http://hz.nwbrower.top/gtfgywpdpb.html

[T32] Lua：局部变量
来源：http://hz.hywenlv.cn/gtqxnzymux.html

local a = 1
来源：http://hz.wangdashe.top/gteioozfvr.html

[T33] Lua：表（数组）
来源：http://hz.gogol.net.cn/gtqgvfvqnm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xuanzx.com/gtbrsyawzo.html

[T34] Lua：遍历表
来源：http://hz.cashguo.top/gtxdxgiqyu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.aizwys.cn/gtdnschrol.html

[T35] Lua：字典表
来源：http://hz.svipenyu.cn/gtootuuyqk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ydzc1.top/gtdylahybi.html

[T36] Lua：函数
来源：http://hz.hnxiangtu.top/gtjqjzedue.html

function add(a, b) return a + b end
来源：http://hz.fzhhl.top/gtbnlbdgdu.html

[T37] Lua：字符串拼接
来源：http://hz.hongshengwenyu.top/gtstrliuay.html

"a" .. "b"
来源：http://hz.jlsjyb.cn/gtjveeohut.html

[T38] Lua：条件
来源：http://hz.xinyue.icu/gtifistugl.html

if x > 0 then print("正") end
来源：http://hz.mhx1999.top/gtplfyqlat.html

[T39] Lua：模式匹配
来源：http://hz.fzhhl.top/gtmlufwecw.html

string.find(s, "%d+")
来源：http://hz.bjfxy.top/gtmoxcporx.html

[T40] Lua：元表
来源：http://hz.tanke756.top/gtcxgyogui.html

setmetatable({}, { __index = base })
来源：http://hz.shzxlz.cn/gtlgrznlyr.html

[T41] Perl：Hello World
来源：http://hz.ydzc1.top/gtvoiartxw.html

print "Hello\n";
来源：http://hz.guannengcc.top/gtaarpayml.html

[T42] Perl：变量类型
来源：http://hz.sysykeji.top/gtfbyejtke.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhixingplan.top/gtzvyvrvbf.html

[T43] Perl：字符串插值
来源：http://hz.hongshengwenyu.top/gtzzfblgcg.html

"值: $a"
来源：http://hz.zhiwuduotai.top/gtlskxyiub.html

[T44] Perl：条件
来源：http://hz.hysaishi.cn/gthfnqggyq.html

if ($a > 0) { print "正"; }
来源：http://hz.shanyushiyangtech.top/gtnvgouafj.html

[T45] Perl：数组遍历
来源：http://hz.jianghu66.top/gtvybruxim.html

for my $x (@arr) { print $x; }
来源：http://hz.svipenyu.cn/gtpjvszvxl.html

[T46] Perl：哈希操作
来源：http://hz.pycfn.com/gtuukkqynv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hongshengwenyu.top/gtjewecivs.html

[T47] Perl：正则捕获
来源：http://hz.havefunace.top/gtqjdlocaw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinqigufen.top/gtpvlgifma.html

[T48] Perl：正则替换
来源：http://hz.hongshengwenyu.top/gtslckgdxc.html

$s =~ s/old/new/g;
来源：http://hz.cheryme.top/gtwnnbgqfl.html

[T49] Perl：函数
来源：http://hz.daria6918.cn/gtgcqtaxrg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hnqzz.top/gtrrpsdvoe.html

[T50] Perl：逐行读文件
来源：http://hz.316326.xyz/gthoizlxgs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhixingplan.top/gtzqdrxnue.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jyoumei.cn/gtdsrrdlxu.html

[T51] Scala：Hello World
来源：http://hz.hnqzz.top/gtbqlpjgjd.html

println("Hello")
来源：http://hz.9152youxi.cn/gtgmlrcaje.html

[T52] Scala：变量
来源：http://hz.zhijiandao.cn/gtwkypocgp.html

val a = 1;  var b = 2
来源：http://hz.wangshuangyany.cn/gtfdibbafg.html

[T53] Scala：字符串插值
来源：http://hz.iojbl.cn/gticpsfcbu.html

s"值: $b"
来源：http://hz.quarkkingdee.top/gttwpkmqjb.html

[T54] Scala：集合映射
来源：http://hz.yonumen.top/gtsrmhqvvz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.316326.xyz/gtghbbkbmo.html

[T55] Scala：集合过滤
来源：http://hz.vqdsnc.cn/gtkweezkuk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhijiandao.cn/gtcrhdwbfk.html

[T56] Scala：样例类
来源：http://hz.sufxvd.cn/gtuddozajv.html

case class User(name: String, age: Int)
来源：http://hz.ydzc1.top/gtvfhaswmu.html

[T57] Scala：模式匹配
来源：http://hz.zhoulong.xyz/gtyysgyatk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.9152youxi.cn/gtvszsqlkv.html

[T58] Scala：函数定义
来源：http://hz.tianlin.xyz/gtslwwoskd.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinyuanbaomall.cn/gtmajzhrjh.html

[T59] Scala：循环
来源：http://hz.yangfankeji.com/gtkzrfkkct.html

for (i <- 1 to 10) println(i)
来源：http://hz.iojbl.cn/gtfvuscuyz.html

[T60] Scala：折叠
来源：http://hz.aibaodan.cn/gtjsanlutb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cucudq.cn/gtwfamsepz.html

================================================================================
来源：http://hz.yvedp.cn/gtqjtauxfg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.smart0.xyz/gtxetnzhft.html

================================================================================
来源：http://hz.zhoulong.xyz/gtujtvvret.html

[U01] Py：创建虚拟环境
来源：http://hz.hammf.cn/gtnyuczcmy.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.9152youxi.cn/gtpswccjcl.html

[U02] Py：导出 / 安装依赖
来源：http://hz.iojbl.cn/gtjtihsntd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hfpthk.cn/gtnotuzuym.html

[U03] Py：加载 .env 配置
来源：http://hz.zycfv.cn/gttconugze.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zdqjudy.top/gtxpbjptcw.html

[U04] Py：变量调试打印
来源：http://hz.c1oappe.top/gtgflbcubk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sweek.top/gtmcwgdcsp.html

[U05] Py：列表去重且保序
来源：http://hz.yvedp.cn/gtmxfjvnjg.html

list(dict.fromkeys(arr))
来源：http://hz.xylfe.cn/gtmfjcqbqx.html

[U06] Py：合并两个字典
来源：http://hz.gaohongyu789.top/gtzyzcprbu.html

{**a, **b}
来源：http://hz.yj202588.top/gtbxztqoft.html

[U07] Py：反转字典键值
来源：http://hz.xziqi.cn/gttsdybafi.html

{v: k for k, v in d.items()}
来源：http://hz.316326.xyz/gtryxykfzu.html

[U08] Py：展平二维列表
来源：http://hz.shanyushiyangtech.top/gtizvorwxk.html

[y for x in nested for y in x]
来源：http://hz.yonumen.top/gtauqislrj.html

[U09] Py：字典取最大值的键
来源：http://hz.chenjidiqi.icu/gtodzegsdv.html

max(d, key=d.get)
来源：http://hz.zhaomingkeji.xyz/gtymbsfxze.html

[U10] Py：按值排序字典
来源：http://hz.xingfuxueyuan.xyz/gtpozobncq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cqqwz.cn/gtyijqeolg.html

[U11] Py：生成器表达式
来源：http://hz.hfpthk.cn/gtovnbalrq.html

(x * 2 for x in arr)
来源：http://hz.316326.xyz/gtibnepqpp.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhongyouzk.top/gtkqdtvpxa.html

Counter(arr).most_common(3)
来源：http://hz.birdmap.top/gtgzadfnzx.html

[U13] Py：固定长度队列
来源：http://hz.mhx1999.top/gtxkvrppot.html

deque(maxlen=10)
来源：http://hz.yueranfly.top/gtlczxauhc.html

[U14] Py：分组收集到列表
来源：http://hz.snrcjt.cn/gtglwyhygy.html

defaultdict(list)
来源：http://hz.guowangkeji.top/gtkfmmyiev.html

[U15] Py：高精度计时
来源：http://hz.gzhubu.top/gtwpmxkenj.html

t = time.perf_counter()
来源：http://hz.gogol.net.cn/gtxluvhrzd.html

[U16] Py：命令行参数解析
来源：http://hz.sufxvd.cn/gtighfogfu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gotoacloud.top/gtoslcscww.html

[U17] Py：初始化日志
来源：http://hz.9152youxi.cn/gtsqovgmld.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.fzhhl.top/gtlfepwafm.html

[U18] Py：预编译正则
来源：http://hz.iojbl.cn/gtunrngxle.html

pat = re.compile(r"\d+")
来源：http://hz.shanyushiyangtech.top/gthtbkuefw.html

[U19] Py：正则替换带回调
来源：http://hz.yuanzhike.top/gtqotgkcwg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cashguo.top/gtcwvcmduv.html

[U20] Py：缓存函数结果
来源：http://hz.yonumen.top/gtqulfscyq.html

@functools.lru_cache(maxsize=None)
来源：http://hz.feifeiyinyue.top/gtkiqkdmec.html

[U21] Py：自定义上下文管理器
来源：http://hz.c1oappe.top/gtgyljvlhl.html

@contextlib.contextmanager
来源：http://hz.zycfv.cn/gthuadwbyl.html

[U22] Py：矩阵转置
来源：http://hz.jinyuanbaomall.cn/gtluleuztk.html

list(zip(*m))
来源：http://hz.zhijiandao.cn/gtzpxyarhi.html

[U23] Py：分块读取大文件
来源：http://hz.zhijiandao.cn/gtzgrzcaoq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.svipenyu.cn/gtdibjcxkw.html

[U24] Py：路径操作
来源：http://hz.sxryk.cn/gtpfxsognh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.daxiang520.top/gtltffzakg.html

[U25] Py：CSV 按字典读
来源：http://hz.haohaochexian.top/gthpubsepm.html

csv.DictReader(f)
来源：http://hz.yangfankeji.com/gtghzxvomb.html

[U26] Py：并发下载
来源：http://hz.xziqi.cn/gttvmywlme.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.fzhhl.top/gtcnaephqd.html

[U27] Py：异步 HTTP
来源：http://hz.cheryme.top/gtmzhedjll.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.nanxinkj.top/gtxzrgffxa.html

[U28] Py：类型别名
来源：http://hz.nanxinkj.top/gtrfcxpodo.html

UserId = int
来源：http://hz.nanxinkj.top/gttxtsoapi.html

[U29] Py：属性校验
来源：http://hz.sxryk.cn/gtaihemtuh.html

@property 与 @x.setter 配合
来源：http://hz.52xcode.cn/gtzxhnmusf.html

[U30] Py：数据类
来源：http://hz.gotoacloud.top/gtrdlpevgi.html

@dataclass(slots=True)
来源：http://hz.zdqjudy.top/gtrggzfgza.html

[U31] Py：单测
来源：http://hz.chenzaomai.com/gtlfvawdzw.html

python -m pytest -q
来源：http://hz.svipenyu.cn/gtzvqdfrfd.html

[U32] Py：代码格式化
来源：http://hz.cheryme.top/gtfkqijraf.html

ruff format . && ruff check --fix .
来源：http://hz.kuanghao11.cn/gtmrafdkbl.html

[U33] Py：打包发布
来源：http://hz.daria6918.cn/gtumcpillb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhixingplan.top/gtqhbphfnt.html

[U34] Py：判断编码
来源：http://hz.jinghuilouyu.cn/gtlnsnyrub.html

chardet.detect(raw)
来源：http://hz.tian-w.cn/gtetyduwqf.html

[U35] Py：发送邮件
来源：http://hz.xylfe.cn/gtwlixyrdw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yuxming.cn/gtbfnotckl.html

[U36] Py：定时任务
来源：http://hz.aibaodan.cn/gtkllubylj.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj20258.top/gtdgahqrxt.html

[U37] Py：读写 Excel
来源：http://hz.jlsjyb.cn/gtqlcpqhue.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.tanke756.top/gteicyvzzq.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhoulong.xyz/gthdzczwcu.html

Path(__file__).resolve().parent
来源：http://hz.yvedp.cn/gtfawvuwxz.html

[U39] Py：判断是否在交互环境
来源：http://hz.bjfxy.top/gthfnsbwxv.html

sys.stdout.isatty()
来源：http://hz.gaohongyu789.top/gtmcnxyycb.html

[U40] Py：打印到标准错误
来源：http://hz.0kj1m.cn/gtxhonkboq.html

print("err", file=sys.stderr)
来源：http://hz.jinghuilouyu.cn/gtkypluerz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cashguo.top/gtxoijbthc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jyoumei.cn/gtxctyuuon.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yangfankeji.com/gtcxdwsptt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ywan-chungtsiang.top/gteumlkutj.html

[U43] PHP：声明命名空间
来源：http://hz.shanyushiyangkeji.top/gtjauxmptb.html

namespace App\Http;
来源：http://hz.pycfn.com/gtvgehfmww.html

[U44] PHP：开启严格类型
来源：http://hz.yonumen.top/gteykctpjt.html

declare(strict_types=1);
来源：http://hz.wangshuangyany.cn/gtpafzviik.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jiagoushi.top/gtszpzsxmt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtfdjcgbtt.html

[U46] PHP：可空类型
来源：http://hz.nwbrower.top/gtpxtfkxwg.html

?string $name = null
来源：http://hz.fengsongda.top/gtfkmneyge.html

[U47] PHP：联合类型
来源：http://hz.yvedp.cn/gtdriaygcn.html

int|string $id
来源：http://hz.chenlongwang.top/gtoxrdrrlp.html

[U48] PHP：纯枚举
来源：http://hz.ehwqpu.com/gtazjeqdcc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhengqikj.top/gtexhlwoqx.html

[U49] PHP：只读属性
来源：http://hz.jinyuanbaomall.cn/gtfnehtcck.html

public readonly string $name
来源：http://hz.hywenlv.cn/gthkawbian.html

[U50] PHP：构造器属性提升
来源：http://hz.pycfn.com/gtnhipdeof.html

public function __construct(private int $id) {}
来源：http://hz.birdmap.top/gtsrkqqsfy.html

[U51] PHP：数组解构
来源：http://hz.jlsjyb.cn/gtmpvwhbio.html

[$a, $b] = $arr;
来源：http://hz.yongpay.top/gtknarimhu.html

[U52] PHP：箭头函数
来源：http://hz.xinyue.icu/gtmyhubblr.html

$double = fn($x) => $x * 2;
来源：http://hz.ywan-chungtsiang.top/gtkvdgwnch.html

[U53] PHP：空合并运算符
来源：http://hz.sxryk.cn/gtpmdzfked.html

$v = $a ?? $b ?? "default";
来源：http://hz.jlsjyb.cn/gticcdynuz.html

[U54] PHP：空安全调用
来源：http://hz.hnqzz.top/gtenbcasrw.html

$obj?->method()
来源：http://hz.hysaishi.cn/gtbcwjutyl.html

[U55] PHP：match 表达式
来源：http://hz.sysykeji.top/gtxeqblvti.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shuidangran.top/gtiisnbjou.html

[U56] PHP：命名参数
来源：http://hz.zhaomingkeji.xyz/gthrtyltte.html

f(a: 1, b: 2)
来源：http://hz.hammf.cn/gtkbitpyic.html

[U57] PHP：字符串插值
来源：http://hz.yueranfly.top/gtbuhhsfjq.html

"值: {$a}"
来源：http://hz.52xcode.cn/gtsepqvqar.html

[U58] PHP：数组三件套
来源：http://hz.jianghu66.top/gtijtgqqsk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zdqjudy.top/gtspwfkmcv.html

[U59] PHP：自定义排序
来源：http://hz.jinyuanbaomall.cn/gtnytflvlz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.wangdashe.top/gtddfebyzk.html

[U60] PHP：JSON 编解码
来源：http://hz.tianlin.xyz/gtgbvohxhk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.316326.xyz/gtehljvtqk.html

[U61] PHP：正则
来源：http://hz.wangdashe.top/gtovhgskuo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.52xcode.cn/gtiljnipmu.html

[U62] PHP：日期对象
来源：http://hz.yongpay.top/gtcxmbfnhv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hysaishi.cn/gtvqjbghcn.html

[U63] PHP：文件读写
来源：http://hz.shanyushiyangkeji.top/gtkxozxvvw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.svipenyu.cn/gtgvpwobtt.html

[U64] PHP：目录遍历
来源：http://hz.zhijiandao.cn/gtyzuiioze.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hywenlv.cn/gtorqcdszu.html

[U65] PHP：会话
来源：http://hz.feifeiyinyue.top/gtkhitqbaz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.haohaochexian.top/gteggtkxgw.html

[U66] PHP：设置 Cookie
来源：http://hz.feifeiyinyue.top/gtznxtdzim.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.snrcjt.cn/gtyoojshkh.html

[U67] PHP：处理文件上传
来源：http://hz.hnqzz.top/gtlkhhfzum.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.dashuyun.cn/gtdgaukwmz.html

[U68] PHP：PDO 连接
来源：http://hz.hongshengwenyu.top/gtjikygxwj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.gzhubu.top/gtxydvxqjv.html

[U69] PHP：PDO 预处理
来源：http://hz.sysykeji.top/gtmerxgqbr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.sxryk.cn/gtdzctikmi.html

[U70] PHP：PDO 事务
来源：http://hz.sweek.top/gtkrzstvjt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cqqwz.cn/gtgcremkub.html

[U71] PHP：抛出异常
来源：http://hz.jinqigfzy.top/gtdpoodgve.html

throw new RuntimeException("失败", 500);
来源：http://hz.yueranfly.top/gtzmqzborc.html

[U72] PHP：写错误日志
来源：http://hz.hfpthk.cn/gtagvmozyl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hfpthk.cn/gtnbzoknfy.html

[U73] PHP：读取 ini 配置
来源：http://hz.quarkkingdee.top/gtskjwuvfg.html

parse_ini_file("config.ini", true)
来源：http://hz.cdnleiting.top/gtknoyfgem.html

[U74] PHP：读取环境变量
来源：http://hz.zhoulong.xyz/gtsokwaocl.html

getenv("APP_ENV") ?: "production"
来源：http://hz.chenlongwang.top/gtfdloeese.html

[U75] PHP：依赖注入
来源：http://hz.daria6918.cn/gtjlsinkwo.html

composer require psr/container
来源：http://hz.sysykeji.top/gtmcvmyive.html

[U76] PHP：简单路由
来源：http://hz.andypj.xyz/gtidnydkno.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shangyingyoupin.top/gtmaglxzeh.html

[U77] PHP：模板渲染
来源：http://hz.pengpengdd.cyou/gtogurzeen.html

composer require twig/twig
来源：http://hz.jyoumei.cn/gtpjxdtnvt.html

[U78] PHP：单元测试
来源：http://hz.cqqwz.cn/gthfhsbgar.html

composer require --dev phpunit/phpunit
来源：http://hz.daxiang520.top/gtdjskhrjg.html

[U79] PHP：静态分析
来源：http://hz.haohaochexian.top/gtnobokcqi.html

composer require --dev phpstan/phpstan
来源：http://hz.vqdsnc.cn/gtykhmgbog.html

[U80] PHP：代码规范修复
来源：http://hz.gogol.net.cn/gtxnjjpgqj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.pycfn.com/gtqwbyylew.html

[U81] JS：初始化项目
来源：http://hz.hnqzz.top/gtmtpwkldw.html

npm init -y;  npm i express
来源：http://hz.xinyue.icu/gtabnomkkc.html

[U82] JS：package.json 脚本
来源：http://hz.zycfv.cn/gtnqxbzrlm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hnqzz.top/gtujobgcpr.html

[U83] JS：ES Module 导入导出
来源：http://hz.wangdashe.top/gtvqmzxmbz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cucudq.cn/gtvaezjqgv.html

[U84] JS：CommonJS 写法
来源：http://hz.dianchejie.cn/gtbacqpkdy.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.bjfxy.top/gtzhuvdzdc.html


<!-- 参考信息 -->