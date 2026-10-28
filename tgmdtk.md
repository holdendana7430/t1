代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.bjfxy.top/gtbpaeznpk.html

[S55] C++：结构化绑定
来源：http://hz.yuanzhike.top/gtgobvowvn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.dashuyun.cn/gtrmfdtgzb.html

[S56] C++：optional
来源：http://hz.shzxlz.cn/gtuwrulqid.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shanyushiyangtech.top/gtiwzxlqrj.html

[S57] C++：编译期常量
来源：http://hz.kuanghao11.cn/gtqdffovpb.html

constexpr int N = 10;
来源：http://hz.zhiwuduotai.top/gttyvrndnm.html

[S58] C++：命名空间
来源：http://hz.jinqigufen.top/gtdpdcwxii.html

namespace ns { int f() { return 1; } }
来源：http://hz.ehwqpu.com/gtqqlhxkmh.html

[S59] C++：静态断言
来源：http://hz.yangfankeji.com/gtdlhvwlmv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxuanxn.top/gttlmrxjkv.html

[S60] C++：遍历并删除元素
来源：http://hz.tian-w.cn/gtwumcmjuj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigfzy.top/gtvbjncllc.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtrfpukzup.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.birdmap.top/gtygxeybow.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtrduiouan.html

[T01] Kotlin：Hello World
来源：http://hz.xinyue.icu/gtqtnwnbpd.html

println("Hello")
来源：http://hz.yonumen.top/gtplnzjywm.html

[T02] Kotlin：变量
来源：http://hz.shanyushiyangtech.top/gtixpfmyji.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hnxiangtu.top/gtnsylgzxj.html

[T03] Kotlin：字符串模板
来源：http://hz.zdqjudy.top/gtdswgabwd.html

"值: $b"
来源：http://hz.yj20258.top/gtgvvqnnzi.html

[T04] Kotlin：空安全
来源：http://hz.redwolf501.top/gtuhscwsho.html

val n: String? = null;  n?.length
来源：http://hz.cdnleiting.top/gtrrlgtufc.html

[T05] Kotlin：when 表达式
来源：http://hz.ydjk.org.cn/gtahnrvote.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.andypj.xyz/gtyqrtikke.html

[T06] Kotlin：集合映射
来源：http://hz.iojbl.cn/gtqvxgctui.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yvedp.cn/gtahfviuxl.html

[T07] Kotlin：集合过滤
来源：http://hz.0kj1m.cn/gtrxlekyej.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jiagoushi.top/gtxdrqaalu.html

[T08] Kotlin：数据类
来源：http://hz.dashuyun.cn/gtdsyezkvj.html

data class User(val name: String, val age: Int)
来源：http://hz.shuidangran.top/gtybczcopz.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgufenzy.top/gtnsnezanw.html

fun String.exclaim() = this + "!"
来源：http://hz.guowangkeji.top/gttrgfgoig.html

[T10] Kotlin：默认参数
来源：http://hz.shanyushiyangkeji.top/gtymeksdah.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenzaomai.com/gtobpqywni.html

[T11] Kotlin：协程
来源：http://hz.ydjk.org.cn/gtojapqcos.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jlsjyb.cn/gtsmrtjqsu.html

[T12] Kotlin：解构声明
来源：http://hz.havefunace.top/gtdpzdcaae.html

val (a, b) = Pair(1, 2)
来源：http://hz.iojbl.cn/gtoxqylczi.html

[T13] Kotlin：只读 Map
来源：http://hz.vqdsnc.cn/gtdrgbzhem.html

val m = mapOf("a" to 1)
来源：http://hz.cashguo.top/gtfwlfkljd.html

[T14] Kotlin：循环
来源：http://hz.meibo888.top/gtymswvudy.html

for (i in 1..10) println(i)
来源：http://hz.nanxuanxn.top/gtfjordsjy.html

[T15] Kotlin：接口
来源：http://hz.cucudq.cn/gtkvgnnvlj.html

interface Shape { fun area(): Double }
来源：http://hz.aizwys.cn/gtbgjdaosd.html

[T16] Swift：Hello World
来源：http://hz.meibo888.top/gtbfuzvowt.html

print("Hello")
来源：http://hz.shangyingyoupin.top/gtvchfjdzk.html

[T17] Swift：变量与常量
来源：http://hz.316326.xyz/gtommfbrlf.html

var a = 1;  let b = 2
来源：http://hz.hysaishi.cn/gtkmagjkjs.html

[T18] Swift：字符串插值
来源：http://hz.guowangkeji.top/gtgwmaeomg.html

"值: \(b)"
来源：http://hz.cdnleiting.top/gtkedelpnz.html

[T19] Swift：可选绑定
来源：http://hz.ywan-chungtsiang.top/gtomeetwgq.html

if let n = opt { print(n) }
来源：http://hz.9152youxi.cn/gtfrensvkt.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtjhpivrph.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shangyingyoupin.top/gtktfxjync.html

[T21] Swift：遍历
来源：http://hz.jyoumei.cn/gtzykuodcl.html

for x in a { print(x) }
来源：http://hz.cashguo.top/gtqworaajf.html

[T22] Swift：字典
来源：http://hz.gotoacloud.top/gtiswanmht.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.dashuyun.cn/gtgpogjilx.html

[T23] Swift：函数
来源：http://hz.jianghu66.top/gtjvekwvob.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cucudq.cn/gtzqovxhki.html

[T24] Swift：闭包
来源：http://hz.birdmap.top/gtihephqty.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.havefunace.top/gtclvaopkd.html

[T25] Swift：结构体
来源：http://hz.quarkkingdee.top/gtihkmyojl.html

struct P { var x: Int }
来源：http://hz.yj20258.top/gttvoxfkok.html

[T26] Swift：类与重写
来源：http://hz.jlsjyb.cn/gtbscsxwph.html

class A: Base { override func f() {} }
来源：http://hz.c1oappe.top/gtfpngvesq.html

[T27] Swift：错误处理
来源：http://hz.hysaishi.cn/gtluhmrkcl.html

do { try f() } catch { print(error) }
来源：http://hz.guannengcc.top/gtftbeaibb.html

[T28] Swift：枚举
来源：http://hz.ywan-chungtsiang.top/gtbeutwvdu.html

enum Color { case red, green }
来源：http://hz.0kj1m.cn/gttjzleoxh.html

[T29] Swift：guard 提前返回
来源：http://hz.andypj.xyz/gtbbeijujw.html

guard let x = opt else { return }
来源：http://hz.ydzc1.top/gtbwbfrehf.html

[T30] Swift：协议
来源：http://hz.cashguo.top/gtnzokpocf.html

protocol Shape { func area() -> Double }
来源：http://hz.316326.xyz/gtjbxilioa.html

[T31] Lua：Hello World
来源：http://hz.andypj.xyz/gtxgtncrck.html

print("Hello")
来源：http://hz.tanke756.top/gtsvwcosqw.html

[T32] Lua：局部变量
来源：http://hz.bjfxy.top/gtmildxvnu.html

local a = 1
来源：http://hz.ivvv.top/gtgvxtaaly.html

[T33] Lua：表（数组）
来源：http://hz.jianghu66.top/gtgeulgpsp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ywan-chungtsiang.top/gtxhtryazg.html

[T34] Lua：遍历表
来源：http://hz.shangyingyoupin.top/gtbcjpgyvs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenjidiqi.icu/gtbogatbod.html

[T35] Lua：字典表
来源：http://hz.jinyuanbaomall.cn/gtqhnuodzy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.andypj.xyz/gthqwvesax.html

[T36] Lua：函数
来源：http://hz.shuidangran.top/gtgcvcsnqh.html

function add(a, b) return a + b end
来源：http://hz.shanyushiyangtech.top/gtzeyrtnzz.html

[T37] Lua：字符串拼接
来源：http://hz.cheryme.top/gtqhhsatzv.html

"a" .. "b"
来源：http://hz.0kj1m.cn/gtwstxeydo.html

[T38] Lua：条件
来源：http://hz.mhx1999.top/gtihcsbxth.html

if x > 0 then print("正") end
来源：http://hz.jinqigufen.top/gtlwuztitq.html

[T39] Lua：模式匹配
来源：http://hz.svipenyu.cn/gtxigqsvzr.html

string.find(s, "%d+")
来源：http://hz.chenzaomai.com/gteyefigxs.html

[T40] Lua：元表
来源：http://hz.andypj.xyz/gtdgpduffx.html

setmetatable({}, { __index = base })
来源：http://hz.xylfe.cn/gtrwktxfej.html

[T41] Perl：Hello World
来源：http://hz.hywenlv.cn/gtpexoiuxg.html

print "Hello\n";
来源：http://hz.jianghu66.top/gtdsciedps.html

[T42] Perl：变量类型
来源：http://hz.zhijiandao.cn/gtguadcinf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.andypj.xyz/gthigyvkbl.html

[T43] Perl：字符串插值
来源：http://hz.tanke756.top/gtdkpletnf.html

"值: $a"
来源：http://hz.daxiang520.top/gtwwbxvhvp.html

[T44] Perl：条件
来源：http://hz.zhiwuduotai.top/gtcufyiqxr.html

if ($a > 0) { print "正"; }
来源：http://hz.yanxiufei.cn/gtqyumrbsg.html

[T45] Perl：数组遍历
来源：http://hz.ydjk.org.cn/gtqwytjnsj.html

for my $x (@arr) { print $x; }
来源：http://hz.sufxvd.cn/gtccwvotmi.html

[T46] Perl：哈希操作
来源：http://hz.iojbl.cn/gtipvfzdvl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.dianchejie.cn/gthiulsqke.html

[T47] Perl：正则捕获
来源：http://hz.guowangkeji.top/gtkccsecgd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinyuanbaomall.cn/gtixcqhjkg.html

[T48] Perl：正则替换
来源：http://hz.jqgfzy.top/gtkjdomgic.html

$s =~ s/old/new/g;
来源：http://hz.svipenyu.cn/gtqozmnpeh.html

[T49] Perl：函数
来源：http://hz.feifeiyinyue.top/gtaeygvbfb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.fengsongda.top/gtmhofwhdi.html

[T50] Perl：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtlwoyzenq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj20258.top/gthwvezvzh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.redwolf501.top/gtpjrhyjxk.html

[T51] Scala：Hello World
来源：http://hz.wangshuangyany.cn/gtsasofumr.html

println("Hello")
来源：http://hz.yueranfly.top/gtncwgycie.html

[T52] Scala：变量
来源：http://hz.cashguo.top/gtpyfwhwzl.html

val a = 1;  var b = 2
来源：http://hz.ydjk.org.cn/gtzgrjubjj.html

[T53] Scala：字符串插值
来源：http://hz.chenjidiqi.icu/gtlbosgoyk.html

s"值: $b"
来源：http://hz.c1oappe.top/gtijtfoctf.html

[T54] Scala：集合映射
来源：http://hz.jinyuanbaomall.cn/gtbqolgrxl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.chenlongwang.top/gtnqezvzxj.html

[T55] Scala：集合过滤
来源：http://hz.cashguo.top/gtvoneloel.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sweek.top/gtkwydgdvv.html

[T56] Scala：样例类
来源：http://hz.xingfuxueyuan.xyz/gtnxcopitv.html

case class User(name: String, age: Int)
来源：http://hz.havefunace.top/gtcoijmxwp.html

[T57] Scala：模式匹配
来源：http://hz.ivvv.top/gtwkjkqwbh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shuidangran.top/gtrkifvxmn.html

[T58] Scala：函数定义
来源：http://hz.andypj.xyz/gtxxzmqlwf.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhongyouzk.top/gtmjbpbnfc.html

[T59] Scala：循环
来源：http://hz.chenjidiqi.icu/gtiwnfxkxt.html

for (i <- 1 to 10) println(i)
来源：http://hz.aizwys.cn/gtolihfnpy.html

[T60] Scala：折叠
来源：http://hz.zhoulong.xyz/gtbhiddugb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shanyushiyangkeji.top/gtixsuczxu.html

================================================================================
来源：http://hz.shuidangran.top/gtbturtajr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hywenlv.cn/gtrrtkchqu.html

================================================================================
来源：http://hz.ehwqpu.com/gtefecognf.html

[U01] Py：创建虚拟环境
来源：http://hz.hongshengwenyu.top/gtqygeyikl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.wangdashe.top/gtxovnkpiz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.daria6918.cn/gtwbgubbbz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.guannengcc.top/gtrmsukknx.html

[U03] Py：加载 .env 配置
来源：http://hz.shangyingyoupin.top/gtbrauupwi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yueranfly.top/gtqfmkoeac.html

[U04] Py：变量调试打印
来源：http://hz.ivvv.top/gtxlfusjqe.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.wangdashe.top/gtsontwhzh.html

[U05] Py：列表去重且保序
来源：http://hz.jqgufenzy.top/gtawekrrcj.html

list(dict.fromkeys(arr))
来源：http://hz.chenlongwang.top/gtjvlxznzk.html

[U06] Py：合并两个字典
来源：http://hz.shzxlz.cn/gtknszcdvz.html

{**a, **b}
来源：http://hz.tanke756.top/gtehoaxwts.html

[U07] Py：反转字典键值
来源：http://hz.yj20258888.top/gtxjhkfhqu.html

{v: k for k, v in d.items()}
来源：http://hz.iojbl.cn/gtlpkpmvkj.html

[U08] Py：展平二维列表
来源：http://hz.yongpay.top/gtrgiogkhw.html

[y for x in nested for y in x]
来源：http://hz.wangshuangyany.cn/gtqdkjfnlv.html

[U09] Py：字典取最大值的键
来源：http://hz.52xcode.cn/gtdppadseh.html

max(d, key=d.get)
来源：http://hz.jyoumei.cn/gtgzxiivml.html

[U10] Py：按值排序字典
来源：http://hz.aibaodan.cn/gtshlwwsyl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinqigufen.top/gtejjzjvtk.html

[U11] Py：生成器表达式
来源：http://hz.ydzc1.top/gtvodxoexb.html

(x * 2 for x in arr)
来源：http://hz.cheryme.top/gtacrjdnhi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.smart0.xyz/gtluziqivh.html

Counter(arr).most_common(3)
来源：http://hz.pycfn.com/gtjlwiopzu.html

[U13] Py：固定长度队列
来源：http://hz.meibo888.top/gtvomhncbz.html

deque(maxlen=10)
来源：http://hz.ydjk.org.cn/gtvpsfozvz.html

[U14] Py：分组收集到列表
来源：http://hz.jqgufenzy.top/gtztiobwqg.html

defaultdict(list)
来源：http://hz.zhijiandao.cn/gtrzquvpzj.html

[U15] Py：高精度计时
来源：http://hz.gaohongyu789.top/gtyykmxnvp.html

t = time.perf_counter()
来源：http://hz.tianlin.xyz/gtlbqaiwsz.html

[U16] Py：命令行参数解析
来源：http://hz.tianlin.xyz/gtppbvdjog.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.mhx1999.top/gtpevkzxue.html

[U17] Py：初始化日志
来源：http://hz.zhiwuduotai.top/gtuvhmqyxr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.cqqwz.cn/gtdhzrupfz.html

[U18] Py：预编译正则
来源：http://hz.shuidangran.top/gtefrpbebn.html

pat = re.compile(r"\d+")
来源：http://hz.redwolf501.top/gtkwkpzjwk.html

[U19] Py：正则替换带回调
来源：http://hz.xziqi.cn/gtgeolpcuz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xuetiantiany.cn/gtzfvaqeen.html

[U20] Py：缓存函数结果
来源：http://hz.zhiwuduotai.top/gtojzzqhga.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinghuilouyu.cn/gtkbpvtvcp.html

[U21] Py：自定义上下文管理器
来源：http://hz.shuidangran.top/gtvkfrquhs.html

@contextlib.contextmanager
来源：http://hz.yj202588.top/gtjneryfym.html

[U22] Py：矩阵转置
来源：http://hz.52xcode.cn/gtlaasxlxo.html

list(zip(*m))
来源：http://hz.aibaodan.cn/gtwpgfzmcc.html

[U23] Py：分块读取大文件
来源：http://hz.yueranfly.top/gthzcpnjjo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.tianlin.xyz/gtnvgnqfnf.html

[U24] Py：路径操作
来源：http://hz.shuidangran.top/gtnjvnfnbb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hywenlv.cn/gtdzztxgcv.html

[U25] Py：CSV 按字典读
来源：http://hz.yongpay.top/gtonsoqbqh.html

csv.DictReader(f)
来源：http://hz.gaohongyu789.top/gtcstpghdr.html

[U26] Py：并发下载
来源：http://hz.ivvv.top/gtifocdhes.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gaohongyu789.top/gtkoqpjccs.html

[U27] Py：异步 HTTP
来源：http://hz.wangdashe.top/gtkpxrrulu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yueranfly.top/gtofrweljl.html

[U28] Py：类型别名
来源：http://hz.sufxvd.cn/gtjnbaontf.html

UserId = int
来源：http://hz.9152youxi.cn/gttuzfdexx.html

[U29] Py：属性校验
来源：http://hz.shuidangran.top/gtrkqivbfn.html

@property 与 @x.setter 配合
来源：http://hz.pycfn.com/gtcjtqdtpp.html

[U30] Py：数据类
来源：http://hz.fzhhl.top/gtmqkkmssc.html

@dataclass(slots=True)
来源：http://hz.meibo888.top/gtonrfbwqk.html

[U31] Py：单测
来源：http://hz.feifeiyinyue.top/gtzigkpzcn.html

python -m pytest -q
来源：http://hz.daxiang520.top/gtbcbuewis.html

[U32] Py：代码格式化
来源：http://hz.zhongyouzk.top/gtikryvfre.html

ruff format . && ruff check --fix .
来源：http://hz.vqdsnc.cn/gtbjqwmbeo.html

[U33] Py：打包发布
来源：http://hz.fzhhl.top/gtoqatnjmy.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hongshengwenyu.top/gtlyrwaohm.html

[U34] Py：判断编码
来源：http://hz.shanyushiyangtech.top/gtizgdtptl.html

chardet.detect(raw)
来源：http://hz.zhixingplan.top/gtjhbervns.html

[U35] Py：发送邮件
来源：http://hz.wangdashe.top/gtorrehhyv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.vqdsnc.cn/gtxaueffda.html

[U36] Py：定时任务
来源：http://hz.yj20258888.top/gtxrukeuno.html

schedule.every(10).minutes.do(job)
来源：http://hz.shanyushiyangtech.top/gtpghuazjk.html

[U37] Py：读写 Excel
来源：http://hz.ywan-chungtsiang.top/gtquadoqps.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.9152youxi.cn/gtuxygnbjz.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhixingplan.top/gtitnnyrfo.html

Path(__file__).resolve().parent
来源：http://hz.hnqzz.top/gtwvbwjlzq.html

[U39] Py：判断是否在交互环境
来源：http://hz.zdqjudy.top/gtnzbkvfmt.html

sys.stdout.isatty()
来源：http://hz.wangdashe.top/gthlnmvsps.html

[U40] Py：打印到标准错误
来源：http://hz.zhiwuduotai.top/gtuehvhjyz.html

print("err", file=sys.stderr)
来源：http://hz.ywan-chungtsiang.top/gttsepydpp.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cashguo.top/gtlgwkbmpu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hnqzz.top/gttlclpsxk.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shuidangran.top/gtmxzrypak.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.nwbrower.top/gtqmejohvb.html

[U43] PHP：声明命名空间
来源：http://hz.jqgufenzy.top/gtwmtvklwx.html

namespace App\Http;
来源：http://hz.hfpthk.cn/gtcbppgzlt.html

[U44] PHP：开启严格类型
来源：http://hz.chenlongwang.top/gtraztmisi.html

declare(strict_types=1);
来源：http://hz.hnxiangtu.top/gthhptngda.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhiwuduotai.top/gtbwnktzxi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhaomingkeji.xyz/gtxhwngeue.html

[U46] PHP：可空类型
来源：http://hz.c1oappe.top/gtwiixyzfy.html

?string $name = null
来源：http://hz.shuidangran.top/gtxbqujtxf.html

[U47] PHP：联合类型
来源：http://hz.sweek.top/gtxvpoqddh.html

int|string $id
来源：http://hz.fzhhl.top/gtkbqxgapp.html

[U48] PHP：纯枚举
来源：http://hz.zhengqikj.top/gtlfpaygcc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.52xcode.cn/gtxqwxidcs.html

[U49] PHP：只读属性
来源：http://hz.sweek.top/gtouszbjwz.html

public readonly string $name
来源：http://hz.pengpengdd.cyou/gtrhcetzpn.html

[U50] PHP：构造器属性提升
来源：http://hz.chenjidiqi.icu/gttczojkdz.html

public function __construct(private int $id) {}
来源：http://hz.nwbrower.top/gttsllixia.html

[U51] PHP：数组解构
来源：http://hz.ivvv.top/gtkufuuixi.html

[$a, $b] = $arr;
来源：http://hz.shangyingyoupin.top/gtvapihcor.html

[U52] PHP：箭头函数
来源：http://hz.jinqigufen.top/gtqikbzowu.html

$double = fn($x) => $x * 2;
来源：http://hz.havefunace.top/gtqnxqfywu.html

[U53] PHP：空合并运算符
来源：http://hz.daxiang520.top/gtgnsoraqc.html

$v = $a ?? $b ?? "default";
来源：http://hz.dashuyun.cn/gtjiikyitc.html

[U54] PHP：空安全调用
来源：http://hz.hywenlv.cn/gtgsblpulf.html

$obj?->method()
来源：http://hz.pengpengdd.cyou/gtemihkzyw.html

[U55] PHP：match 表达式
来源：http://hz.cashguo.top/gtjbeqrrva.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.c1oappe.top/gttmffmipz.html

[U56] PHP：命名参数
来源：http://hz.jiagoushi.top/gtginfmpac.html

f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtjwfavrsb.html

[U57] PHP：字符串插值
来源：http://hz.9152youxi.cn/gtcwpqfetj.html

"值: {$a}"
来源：http://hz.gzhubu.top/gtmytjzhag.html

[U58] PHP：数组三件套
来源：http://hz.xylfe.cn/gtrpnbijpe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.pengpengdd.cyou/gtdfomslkc.html

[U59] PHP：自定义排序
来源：http://hz.bjfxy.top/gtsxpzhgqa.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhoulong.xyz/gtafpriycg.html

[U60] PHP：JSON 编解码
来源：http://hz.haohaochexian.top/gtsmdbcdnq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yanxiufei.cn/gtxvhyxknf.html

[U61] PHP：正则
来源：http://hz.jqgfzy.top/gtbrzamwqd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jianghu66.top/gtopfzospo.html

[U62] PHP：日期对象
来源：http://hz.hnxiangtu.top/gtkwrsvork.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhengqikj.top/gtexmyocxm.html

[U63] PHP：文件读写
来源：http://hz.cqqwz.cn/gtgjnlccek.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xuanzx.com/gtczvxsmlh.html

[U64] PHP：目录遍历
来源：http://hz.dashuyun.cn/gtudsgmvkh.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.0kj1m.cn/gtyqmtqclo.html

[U65] PHP：会话
来源：http://hz.zhaomingkeji.xyz/gtmgciexef.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ppjwa.cn/gttwfoktnx.html

[U66] PHP：设置 Cookie
来源：http://hz.nanxinkj.top/gtbjkoknep.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.aizwys.cn/gtomktkiyc.html

[U67] PHP：处理文件上传
来源：http://hz.shuidangran.top/gtalwgtmwo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hammf.cn/gtsnbyitws.html

[U68] PHP：PDO 连接
来源：http://hz.vqdsnc.cn/gtzgomquji.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.haohaochexian.top/gtegkcxrwb.html

[U69] PHP：PDO 预处理
来源：http://hz.316326.xyz/gtzrvnryji.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.chenzaomai.com/gtzncpoouj.html

[U70] PHP：PDO 事务
来源：http://hz.cdnleiting.top/gtcieqmdrr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hywenlv.cn/gtyhwreadv.html

[U71] PHP：抛出异常
来源：http://hz.zycfv.cn/gtcvsupnrc.html

throw new RuntimeException("失败", 500);
来源：http://hz.feifeiyinyue.top/gtwkilpkbt.html

[U72] PHP：写错误日志
来源：http://hz.jlsjyb.cn/gtnllxmsuz.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shanyushiyangkeji.top/gtmjufpjti.html

[U73] PHP：读取 ini 配置
来源：http://hz.zycfv.cn/gtxgvibwda.html

parse_ini_file("config.ini", true)
来源：http://hz.jinqigufen.top/gtxdgutfym.html

[U74] PHP：读取环境变量
来源：http://hz.vqdsnc.cn/gtiofmfdwf.html

getenv("APP_ENV") ?: "production"
来源：http://hz.quarkkingdee.top/gtyonyuyps.html

[U75] PHP：依赖注入
来源：http://hz.sxryk.cn/gtuqvxdmvu.html

composer require psr/container
来源：http://hz.zycfv.cn/gtnjszytpy.html

[U76] PHP：简单路由
来源：http://hz.meibo888.top/gtapeoirag.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yj20258.top/gtuaxuvirm.html

[U77] PHP：模板渲染
来源：http://hz.aizwys.cn/gtsezhczso.html

composer require twig/twig
来源：http://hz.hfpthk.cn/gtpooalsrt.html

[U78] PHP：单元测试
来源：http://hz.smart0.xyz/gtraaawkeb.html

composer require --dev phpunit/phpunit
来源：http://hz.zhengqikj.top/gtucawhyyx.html

[U79] PHP：静态分析
来源：http://hz.chenlongwang.top/gtaederfmw.html

composer require --dev phpstan/phpstan
来源：http://hz.havefunace.top/gtkgfnqlht.html

[U80] PHP：代码规范修复
来源：http://hz.hnqzz.top/gtshltiaic.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jinghuilouyu.cn/gtubfalvvn.html


<!-- 参考信息 -->