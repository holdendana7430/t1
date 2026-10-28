代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://hz.cucudq.cn/gteuxmanak.html

[S59] C++：静态断言
来源：http://hz.ehwqpu.com/gtjdegcqch.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cashguo.top/gtdmuhfsht.html

[S60] C++：遍历并删除元素
来源：http://hz.jlsjyb.cn/gtvlpurxcb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sweek.top/gtxkwrkjvf.html

================================================================================
来源：http://hz.snrcjt.cn/gtmvrreczd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tianlin.xyz/gttuwryebe.html

================================================================================
来源：http://hz.hfpthk.cn/gtsparqevw.html

[T01] Kotlin：Hello World
来源：http://hz.jinghuilouyu.cn/gtrbtzdhdk.html

println("Hello")
来源：http://hz.jinghuilouyu.cn/gtbjzyusro.html

[T02] Kotlin：变量
来源：http://hz.cucudq.cn/gtvjrutzbh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cucudq.cn/gtkccbrdhh.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258888.top/gtaqpuzmux.html

"值: $b"
来源：http://hz.sufxvd.cn/gtnlpguhef.html

[T04] Kotlin：空安全
来源：http://hz.yj20258.top/gtwexyqcff.html

val n: String? = null;  n?.length
来源：http://hz.bjfxy.top/gtoayswpne.html

[T05] Kotlin：when 表达式
来源：http://hz.smart0.xyz/gtovgqnegi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.52xcode.cn/gtnoebzmnf.html

[T06] Kotlin：集合映射
来源：http://hz.gzhubu.top/gtezucvkws.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jqgfzy.top/gthqnvedel.html

[T07] Kotlin：集合过滤
来源：http://hz.dianchejie.cn/gtfrlflwxl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.guowangkeji.top/gtcrmswsqk.html

[T08] Kotlin：数据类
来源：http://hz.gzhubu.top/gtlpxkjiqu.html

data class User(val name: String, val age: Int)
来源：http://hz.cashguo.top/gtkawgepxn.html

[T09] Kotlin：扩展函数
来源：http://hz.tian-w.cn/gtozsnfftl.html

fun String.exclaim() = this + "!"
来源：http://hz.redwolf501.top/gtcdmpaajr.html

[T10] Kotlin：默认参数
来源：http://hz.cashguo.top/gtyitiwqrs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xingfuxueyuan.xyz/gtsliemzfs.html

[T11] Kotlin：协程
来源：http://hz.hammf.cn/gtayrmexez.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.birdmap.top/gtyzockiga.html

[T12] Kotlin：解构声明
来源：http://hz.svipenyu.cn/gtopwyejwv.html

val (a, b) = Pair(1, 2)
来源：http://hz.0kj1m.cn/gtxycimunx.html

[T13] Kotlin：只读 Map
来源：http://hz.jinyuanbaomall.cn/gtqmxrxtev.html

val m = mapOf("a" to 1)
来源：http://hz.jinqigufen.top/gtlummbtxk.html

[T14] Kotlin：循环
来源：http://hz.shanyushiyangkeji.top/gtanavgfmr.html

for (i in 1..10) println(i)
来源：http://hz.bjfxy.top/gtupkzlagl.html

[T15] Kotlin：接口
来源：http://hz.xinyue.icu/gtzrrhwyzw.html

interface Shape { fun area(): Double }
来源：http://hz.jinghuilouyu.cn/gtsinisrej.html

[T16] Swift：Hello World
来源：http://hz.52xcode.cn/gtcczqlort.html

print("Hello")
来源：http://hz.jinqigfzy.top/gtfjiiolzu.html

[T17] Swift：变量与常量
来源：http://hz.meibo888.top/gtksiyxfrm.html

var a = 1;  let b = 2
来源：http://hz.sysykeji.top/gtnejlrtmm.html

[T18] Swift：字符串插值
来源：http://hz.yangfankeji.com/gtsbzjgvyl.html

"值: \(b)"
来源：http://hz.yuanzhike.top/gtckwwztsn.html

[T19] Swift：可选绑定
来源：http://hz.ehwqpu.com/gtifxwulku.html

if let n = opt { print(n) }
来源：http://hz.hysaishi.cn/gtraibobts.html

[T20] Swift：数组操作
来源：http://hz.feifeiyinyue.top/gtpjtgzvfs.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.9152youxi.cn/gtidwugwsh.html

[T21] Swift：遍历
来源：http://hz.smart0.xyz/gtowtlmdsu.html

for x in a { print(x) }
来源：http://hz.guowangkeji.top/gteqnewdek.html

[T22] Swift：字典
来源：http://hz.yj20258.top/gtmabdurkt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yj202588.top/gtrmyjdewf.html

[T23] Swift：函数
来源：http://hz.hnqzz.top/gtitktwsqo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cashguo.top/gthregzhga.html

[T24] Swift：闭包
来源：http://hz.zycfv.cn/gteyuhuqqd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jqgfzy.top/gtwubjndzw.html

[T25] Swift：结构体
来源：http://hz.gogol.net.cn/gtoebwwmsg.html

struct P { var x: Int }
来源：http://hz.yvedp.cn/gtivlndxhd.html

[T26] Swift：类与重写
来源：http://hz.chenlongwang.top/gtcgkluxhy.html

class A: Base { override func f() {} }
来源：http://hz.316326.xyz/gtgorcmarg.html

[T27] Swift：错误处理
来源：http://hz.chenlongwang.top/gtyudgnswp.html

do { try f() } catch { print(error) }
来源：http://hz.yangfankeji.com/gtadgamzpz.html

[T28] Swift：枚举
来源：http://hz.yvedp.cn/gtxtcsdeiz.html

enum Color { case red, green }
来源：http://hz.cqqwz.cn/gtokqxgmob.html

[T29] Swift：guard 提前返回
来源：http://hz.iojbl.cn/gtxccpfohz.html

guard let x = opt else { return }
来源：http://hz.316326.xyz/gtsgkiuwsk.html

[T30] Swift：协议
来源：http://hz.xylfe.cn/gtmlyrjihw.html

protocol Shape { func area() -> Double }
来源：http://hz.cheryme.top/gttreoiqzh.html

[T31] Lua：Hello World
来源：http://hz.jyoumei.cn/gtmkobndrl.html

print("Hello")
来源：http://hz.cqqwz.cn/gtgaxpykcs.html

[T32] Lua：局部变量
来源：http://hz.zhijiandao.cn/gtphhxtmdy.html

local a = 1
来源：http://hz.kuanghao11.cn/gtupfekstf.html

[T33] Lua：表（数组）
来源：http://hz.ivvv.top/gtpyvrgrsu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hongshengwenyu.top/gtgoxgacii.html

[T34] Lua：遍历表
来源：http://hz.sxryk.cn/gtjchdvbpy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenlongwang.top/gtmjuwkedr.html

[T35] Lua：字典表
来源：http://hz.shanyushiyangkeji.top/gtvvrejdmt.html

local d = { a = 1 };  d.b = 2
来源：http://hz.meibo888.top/gthozxcegh.html

[T36] Lua：函数
来源：http://hz.yj20258888.top/gtvcjmlobo.html

function add(a, b) return a + b end
来源：http://hz.hfpthk.cn/gtmshuwimx.html

[T37] Lua：字符串拼接
来源：http://hz.zdqjudy.top/gtrzceezmo.html

"a" .. "b"
来源：http://hz.cashguo.top/gtmebaipfc.html

[T38] Lua：条件
来源：http://hz.mhx1999.top/gtpuzrqcil.html

if x > 0 then print("正") end
来源：http://hz.jqgufenzy.top/gtztyhjale.html

[T39] Lua：模式匹配
来源：http://hz.ydjk.org.cn/gtkexciylx.html

string.find(s, "%d+")
来源：http://hz.pycfn.com/gtppjvlmwh.html

[T40] Lua：元表
来源：http://hz.ppjwa.cn/gtkgbgyaim.html

setmetatable({}, { __index = base })
来源：http://hz.zhiwuduotai.top/gtzxxnzbvd.html

[T41] Perl：Hello World
来源：http://hz.havefunace.top/gtumqihlqv.html

print "Hello\n";
来源：http://hz.shanyushiyangkeji.top/gtcgpwvqdz.html

[T42] Perl：变量类型
来源：http://hz.yonumen.top/gtrwzigkhh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.chenzaomai.com/gtionmliij.html

[T43] Perl：字符串插值
来源：http://hz.wangdashe.top/gtodzdvveg.html

"值: $a"
来源：http://hz.pengpengdd.cyou/gtciqghqdp.html

[T44] Perl：条件
来源：http://hz.jinyuanbaomall.cn/gtvbppdayl.html

if ($a > 0) { print "正"; }
来源：http://hz.ppjwa.cn/gtfranirtu.html

[T45] Perl：数组遍历
来源：http://hz.cucudq.cn/gtporszyed.html

for my $x (@arr) { print $x; }
来源：http://hz.ydzc1.top/gtqptxrgwv.html

[T46] Perl：哈希操作
来源：http://hz.zhaomingkeji.xyz/gtdfvgxppb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinqigfzy.top/gtmosfuybd.html

[T47] Perl：正则捕获
来源：http://hz.xinyue.icu/gtrypitqvg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shzxlz.cn/gtfdhnvrwc.html

[T48] Perl：正则替换
来源：http://hz.pengpengdd.cyou/gtkuckdezx.html

$s =~ s/old/new/g;
来源：http://hz.sweek.top/gtdptgayti.html

[T49] Perl：函数
来源：http://hz.zhiwuduotai.top/gtoytlnsqu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtkjhckhch.html

[T50] Perl：逐行读文件
来源：http://hz.haohaochexian.top/gtgzkwjatw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hnxiangtu.top/gtuemwiaph.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xziqi.cn/gtgmdafbpp.html

[T51] Scala：Hello World
来源：http://hz.jinghuilouyu.cn/gtakeddmuq.html

println("Hello")
来源：http://hz.kuanghao11.cn/gtdfmapuzw.html

[T52] Scala：变量
来源：http://hz.tianlin.xyz/gtgxlynrph.html

val a = 1;  var b = 2
来源：http://hz.ybcxt.top/gtmdokqxui.html

[T53] Scala：字符串插值
来源：http://hz.shanyushiyangtech.top/gtdnbkkguu.html

s"值: $b"
来源：http://hz.shzxlz.cn/gtqmjbstyh.html

[T54] Scala：集合映射
来源：http://hz.yueranfly.top/gtdgmnzryd.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.chenjidiqi.icu/gthztxoycd.html

[T55] Scala：集合过滤
来源：http://hz.yuanzhike.top/gtifrdregl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.snrcjt.cn/gtcpfqgmza.html

[T56] Scala：样例类
来源：http://hz.iojbl.cn/gtnulhvwio.html

case class User(name: String, age: Int)
来源：http://hz.yueranfly.top/gtedmmnefm.html

[T57] Scala：模式匹配
来源：http://hz.gaohongyu789.top/gtgknudwmt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ydzc1.top/gthoydvoaa.html

[T58] Scala：函数定义
来源：http://hz.nwbrower.top/gtzrfpyqly.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jianghu66.top/gtidjnguql.html

[T59] Scala：循环
来源：http://hz.dianchejie.cn/gthntygyal.html

for (i <- 1 to 10) println(i)
来源：http://hz.9152youxi.cn/gtrelbwtry.html

[T60] Scala：折叠
来源：http://hz.iojbl.cn/gtphuwtyxa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.redwolf501.top/gtpwusncfz.html

================================================================================
来源：http://hz.yj20258.top/gtqrohpsqg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.vqdsnc.cn/gtavxluhqx.html

================================================================================
来源：http://hz.sxryk.cn/gtnqhbuvko.html

[U01] Py：创建虚拟环境
来源：http://hz.jqgfzy.top/gtosxaiqph.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhijiandao.cn/gtrenhinum.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fengsongda.top/gtsqyyuxye.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ydjk.org.cn/gtncjsqquf.html

[U03] Py：加载 .env 配置
来源：http://hz.sufxvd.cn/gtxxvsiyid.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.9152youxi.cn/gtbokomtmj.html

[U04] Py：变量调试打印
来源：http://hz.jinqigufen.top/gtriyilcak.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shuidangran.top/gtankoasve.html

[U05] Py：列表去重且保序
来源：http://hz.yuxming.cn/gtjorjwpvx.html

list(dict.fromkeys(arr))
来源：http://hz.fengsongda.top/gtrupprsjv.html

[U06] Py：合并两个字典
来源：http://hz.daria6918.cn/gtfhlzbtlz.html

{**a, **b}
来源：http://hz.hnqzz.top/gttfoamjhk.html

[U07] Py：反转字典键值
来源：http://hz.ppjwa.cn/gtsgvzoyyh.html

{v: k for k, v in d.items()}
来源：http://hz.nanxinkj.top/gttqauvsun.html

[U08] Py：展平二维列表
来源：http://hz.hysaishi.cn/gtucbwhniu.html

[y for x in nested for y in x]
来源：http://hz.svipenyu.cn/gtzittjbxu.html

[U09] Py：字典取最大值的键
来源：http://hz.jqgufenzy.top/gtvizdwixe.html

max(d, key=d.get)
来源：http://hz.daria6918.cn/gtbsqcypkd.html

[U10] Py：按值排序字典
来源：http://hz.gzhubu.top/gtjbjbpgrz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dianchejie.cn/gtugqnqjbf.html

[U11] Py：生成器表达式
来源：http://hz.mhx1999.top/gtosoyzfxn.html

(x * 2 for x in arr)
来源：http://hz.zhaomingkeji.xyz/gtijqqynjv.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tanke756.top/gtbgleuhzo.html

Counter(arr).most_common(3)
来源：http://hz.nwbrower.top/gtlwrizdsg.html

[U13] Py：固定长度队列
来源：http://hz.cqqwz.cn/gtayiscgxk.html

deque(maxlen=10)
来源：http://hz.yvedp.cn/gtyospjrbc.html

[U14] Py：分组收集到列表
来源：http://hz.pengpengdd.cyou/gtcpmzvcih.html

defaultdict(list)
来源：http://hz.yongpay.top/gtwxoojuis.html

[U15] Py：高精度计时
来源：http://hz.shuidangran.top/gthvvqisnh.html

t = time.perf_counter()
来源：http://hz.zhongyouzk.top/gtwkleuihy.html

[U16] Py：命令行参数解析
来源：http://hz.hnxiangtu.top/gtizfyrrfc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yj20258.top/gtkdsrupmg.html

[U17] Py：初始化日志
来源：http://hz.fzhhl.top/gtxygmbptn.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.316326.xyz/gtvuorrycw.html

[U18] Py：预编译正则
来源：http://hz.tian-w.cn/gtajhqvuru.html

pat = re.compile(r"\d+")
来源：http://hz.gaohongyu789.top/gtnenhairi.html

[U19] Py：正则替换带回调
来源：http://hz.haohaochexian.top/gthfvmestw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhaomingkeji.xyz/gtmdiemgwc.html

[U20] Py：缓存函数结果
来源：http://hz.zhengqikj.top/gtjxwyezac.html

@functools.lru_cache(maxsize=None)
来源：http://hz.tianlin.xyz/gtfuxppaoa.html

[U21] Py：自定义上下文管理器
来源：http://hz.yuanzhike.top/gtqoldktrf.html

@contextlib.contextmanager
来源：http://hz.shzxlz.cn/gtiqoesxku.html

[U22] Py：矩阵转置
来源：http://hz.smart0.xyz/gtudnhrqdk.html

list(zip(*m))
来源：http://hz.xuetiantiany.cn/gtyhgodxwi.html

[U23] Py：分块读取大文件
来源：http://hz.tian-w.cn/gtpmifjlgk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.guannengcc.top/gtcvwutmpk.html

[U24] Py：路径操作
来源：http://hz.chenjidiqi.icu/gtmkeumtbt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.nanxuanxn.top/gtyrpuvexc.html

[U25] Py：CSV 按字典读
来源：http://hz.andypj.xyz/gtlmqnbreg.html

csv.DictReader(f)
来源：http://hz.sufxvd.cn/gtoctazpjk.html

[U26] Py：并发下载
来源：http://hz.xziqi.cn/gtvkcxunvq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xziqi.cn/gtaukqvwln.html

[U27] Py：异步 HTTP
来源：http://hz.zhaomingkeji.xyz/gtiywexmhe.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shangyingyoupin.top/gtxmztuemn.html

[U28] Py：类型别名
来源：http://hz.ybcxt.top/gtfeaddchw.html

UserId = int
来源：http://hz.cqqwz.cn/gtmhplkkzn.html

[U29] Py：属性校验
来源：http://hz.xuanzx.com/gtzetegwxn.html

@property 与 @x.setter 配合
来源：http://hz.redwolf501.top/gtfbkhdesv.html

[U30] Py：数据类
来源：http://hz.zhongyouzk.top/gtmdjatgbp.html

@dataclass(slots=True)
来源：http://hz.sweek.top/gtqzdwilbj.html

[U31] Py：单测
来源：http://hz.meibo888.top/gtamupbgzi.html

python -m pytest -q
来源：http://hz.yanxiufei.cn/gtisgpyzoh.html

[U32] Py：代码格式化
来源：http://hz.shanyushiyangtech.top/gteuijbnpr.html

ruff format . && ruff check --fix .
来源：http://hz.tian-w.cn/gtlbrgkwvt.html

[U33] Py：打包发布
来源：http://hz.shangyingyoupin.top/gtlrdlitde.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gaohongyu789.top/gtorpkxpzs.html

[U34] Py：判断编码
来源：http://hz.cqqwz.cn/gtujgnjqhb.html

chardet.detect(raw)
来源：http://hz.fengsongda.top/gtdlydmssu.html

[U35] Py：发送邮件
来源：http://hz.jqgufenzy.top/gttpqnawiw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.aizwys.cn/gtayygzxpi.html

[U36] Py：定时任务
来源：http://hz.zycfv.cn/gtexyxrnyl.html

schedule.every(10).minutes.do(job)
来源：http://hz.mhx1999.top/gtobjmqlyy.html

[U37] Py：读写 Excel
来源：http://hz.pengpengdd.cyou/gtodukwlxi.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hysaishi.cn/gtjwddkewi.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhengqikj.top/gtrzeiihsm.html

Path(__file__).resolve().parent
来源：http://hz.0kj1m.cn/gtsftvsugd.html

[U39] Py：判断是否在交互环境
来源：http://hz.yueranfly.top/gttaaocdli.html

sys.stdout.isatty()
来源：http://hz.chenjidiqi.icu/gtjmrmmsid.html

[U40] Py：打印到标准错误
来源：http://hz.zhijiandao.cn/gtlltxxzid.html

print("err", file=sys.stderr)
来源：http://hz.jiagoushi.top/gtdugaagbr.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.52xcode.cn/gtdybrydyh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.nanxuanxn.top/gtyboqeosd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.pycfn.com/gtjgwbcaxe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.aizwys.cn/gtxdetbdvm.html

[U43] PHP：声明命名空间
来源：http://hz.snrcjt.cn/gtpxksemsi.html

namespace App\Http;
来源：http://hz.bjfxy.top/gtfsszksrp.html

[U44] PHP：开启严格类型
来源：http://hz.guannengcc.top/gtfxgctyxv.html

declare(strict_types=1);
来源：http://hz.c1oappe.top/gtitlhlwjt.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hysaishi.cn/gtfqxttozu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtinlubjkv.html

[U46] PHP：可空类型
来源：http://hz.hongshengwenyu.top/gtcryunamp.html

?string $name = null
来源：http://hz.316326.xyz/gtkauvxubx.html

[U47] PHP：联合类型
来源：http://hz.hnxiangtu.top/gtsrfzzemf.html

int|string $id
来源：http://hz.jinqigfzy.top/gtenccgdsu.html

[U48] PHP：纯枚举
来源：http://hz.zhiwuduotai.top/gtctgcosjq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinyuanbaomall.cn/gtfaebivgn.html

[U49] PHP：只读属性
来源：http://hz.jlsjyb.cn/gtribuzxjg.html

public readonly string $name
来源：http://hz.sweek.top/gtofylidqi.html

[U50] PHP：构造器属性提升
来源：http://hz.zhongyouzk.top/gtrpyxmkfx.html

public function __construct(private int $id) {}
来源：http://hz.nwbrower.top/gttlluapty.html

[U51] PHP：数组解构
来源：http://hz.daxiang520.top/gtikqkjhvd.html

[$a, $b] = $arr;
来源：http://hz.guowangkeji.top/gtsklciylk.html

[U52] PHP：箭头函数
来源：http://hz.zhixingplan.top/gtkhbcvtld.html

$double = fn($x) => $x * 2;
来源：http://hz.haohaochexian.top/gtjoybukag.html

[U53] PHP：空合并运算符
来源：http://hz.iojbl.cn/gtxdivwidh.html

$v = $a ?? $b ?? "default";
来源：http://hz.daria6918.cn/gtzotxomwn.html

[U54] PHP：空安全调用
来源：http://hz.nanxinkj.top/gtelanfxra.html

$obj?->method()
来源：http://hz.316326.xyz/gturuiujmz.html

[U55] PHP：match 表达式
来源：http://hz.jqgufenzy.top/gthkncwkwy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jqgfzy.top/gtnlyavvxa.html

[U56] PHP：命名参数
来源：http://hz.zhongyouzk.top/gtqsjtshan.html

f(a: 1, b: 2)
来源：http://hz.meibo888.top/gtldnaotmh.html

[U57] PHP：字符串插值
来源：http://hz.iojbl.cn/gtgbzgjtvl.html

"值: {$a}"
来源：http://hz.havefunace.top/gtpedmheks.html

[U58] PHP：数组三件套
来源：http://hz.gotoacloud.top/gtqjidywek.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zdqjudy.top/gtwzzlzgwt.html

[U59] PHP：自定义排序
来源：http://hz.zhongyouzk.top/gtibjgpseo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ppjwa.cn/gtngumfpnt.html

[U60] PHP：JSON 编解码
来源：http://hz.dianchejie.cn/gtesqaqetu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj20258.top/gtcadiwoit.html

[U61] PHP：正则
来源：http://hz.hnqzz.top/gtziwngugz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.aizwys.cn/gtlnxiawwi.html

[U62] PHP：日期对象
来源：http://hz.zhiwuduotai.top/gtnbkqdgjb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hnqzz.top/gtcstwvivt.html

[U63] PHP：文件读写
来源：http://hz.guannengcc.top/gtmpywlqep.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.fzhhl.top/gtcybniquv.html

[U64] PHP：目录遍历
来源：http://hz.c1oappe.top/gtndjrxkpn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.shanyushiyangtech.top/gtzvrszqsb.html

[U65] PHP：会话
来源：http://hz.sysykeji.top/gtwjktprvm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shuidangran.top/gtkdylxoub.html

[U66] PHP：设置 Cookie
来源：http://hz.nanxuanxn.top/gtisgjafsp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.quarkkingdee.top/gtwmtokell.html

[U67] PHP：处理文件上传
来源：http://hz.feifeiyinyue.top/gtwtmzfygt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhijiandao.cn/gteeltjqlk.html

[U68] PHP：PDO 连接
来源：http://hz.yueranfly.top/gtjuorikbx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yuanzhike.top/gtisotsyda.html

[U69] PHP：PDO 预处理
来源：http://hz.shuidangran.top/gtamjhzkrh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gogol.net.cn/gtfymovyyx.html

[U70] PHP：PDO 事务
来源：http://hz.yj202588.top/gtludbdcpb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zycfv.cn/gtpxeslamn.html

[U71] PHP：抛出异常
来源：http://hz.xziqi.cn/gtmnnblxbp.html

throw new RuntimeException("失败", 500);
来源：http://hz.pengpengdd.cyou/gtaxefwxvl.html

[U72] PHP：写错误日志
来源：http://hz.ydzc1.top/gtsncteauc.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jqgfzy.top/gttgpqxndt.html

[U73] PHP：读取 ini 配置
来源：http://hz.ivvv.top/gtpznjthfo.html

parse_ini_file("config.ini", true)
来源：http://hz.mhx1999.top/gtakywdnbq.html

[U74] PHP：读取环境变量
来源：http://hz.shanyushiyangkeji.top/gtpipmzvzq.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhongyouzk.top/gtufemrwzv.html

[U75] PHP：依赖注入
来源：http://hz.chenjidiqi.icu/gtrqerhsjn.html

composer require psr/container
来源：http://hz.0kj1m.cn/gtgdqizbve.html

[U76] PHP：简单路由
来源：http://hz.ppjwa.cn/gtprnvzqjy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jinyuanbaomall.cn/gtmrogjwoo.html

[U77] PHP：模板渲染
来源：http://hz.jianghu66.top/gtjiswpvkg.html

composer require twig/twig
来源：http://hz.shangyingyoupin.top/gtjgzcjuta.html

[U78] PHP：单元测试
来源：http://hz.fzhhl.top/gtwcjfqcqx.html

composer require --dev phpunit/phpunit
来源：http://hz.cqqwz.cn/gtnglwlasw.html

[U79] PHP：静态分析
来源：http://hz.pycfn.com/gtejnxmmkb.html

composer require --dev phpstan/phpstan
来源：http://hz.yanxiufei.cn/gtiqywguyt.html

[U80] PHP：代码规范修复
来源：http://hz.zhijiandao.cn/gtlfhrcmlh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xuanzx.com/gthabnadnr.html

[U81] JS：初始化项目
来源：http://hz.sysykeji.top/gtldvjrawu.html

npm init -y;  npm i express
来源：http://hz.jqgufenzy.top/gtmpulezbi.html

[U82] JS：package.json 脚本
来源：http://hz.ydzc1.top/gtgcykibzb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yj202588.top/gtagwlzkpc.html

[U83] JS：ES Module 导入导出
来源：http://hz.fzhhl.top/gtbbrphfib.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.tanke756.top/gtaczbwual.html

[U84] JS：CommonJS 写法
来源：http://hz.hysaishi.cn/gtjsmpgcfa.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yj20258888.top/gthcvnxptt.html


<!-- 参考信息 -->