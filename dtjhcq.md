代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guowangkeji.top/gtyjiudsnp.html

[S55] C++：结构化绑定
来源：http://hz.0kj1m.cn/gtuimpyeao.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xuanzx.com/gtfrpasmkg.html

[S56] C++：optional
来源：http://hz.zhixingplan.top/gttypknlvz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.9152youxi.cn/gtqbuswzwp.html

[S57] C++：编译期常量
来源：http://hz.guannengcc.top/gtjypcotry.html

constexpr int N = 10;
来源：http://hz.chenlongwang.top/gtiqlhunxw.html

[S58] C++：命名空间
来源：http://hz.aibaodan.cn/gttukwdlil.html

namespace ns { int f() { return 1; } }
来源：http://hz.c1oappe.top/gtzvluwwtb.html

[S59] C++：静态断言
来源：http://hz.sweek.top/gtaolczavf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fengsongda.top/gtowmomcqp.html

[S60] C++：遍历并删除元素
来源：http://hz.wangshuangyany.cn/gtslyuvpnb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cheryme.top/gtrxrslent.html

================================================================================
来源：http://hz.hywenlv.cn/gtricnrlkb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daxiang520.top/gtyhjyrgnb.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtriluyypl.html

[T01] Kotlin：Hello World
来源：http://hz.daria6918.cn/gtaquiqjwh.html

println("Hello")
来源：http://hz.aizwys.cn/gttupombxc.html

[T02] Kotlin：变量
来源：http://hz.chenjidiqi.icu/gtdwaijtmc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxuanxn.top/gtxawwmayk.html

[T03] Kotlin：字符串模板
来源：http://hz.jlsjyb.cn/gtrsbgahur.html

"值: $b"
来源：http://hz.xuanzx.com/gtnoppcnrx.html

[T04] Kotlin：空安全
来源：http://hz.yj20258888.top/gttqlpyvsg.html

val n: String? = null;  n?.length
来源：http://hz.ppjwa.cn/gtjquuqbft.html

[T05] Kotlin：when 表达式
来源：http://hz.cashguo.top/gtikvkokxv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.daria6918.cn/gtwezycztt.html

[T06] Kotlin：集合映射
来源：http://hz.yvedp.cn/gtxzduwdxw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinghuilouyu.cn/gtiujgzrje.html

[T07] Kotlin：集合过滤
来源：http://hz.dashuyun.cn/gtsshkakio.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cdnleiting.top/gtbzcokhha.html

[T08] Kotlin：数据类
来源：http://hz.nanxuanxn.top/gtlnobnatz.html

data class User(val name: String, val age: Int)
来源：http://hz.haohaochexian.top/gtddiomyes.html

[T09] Kotlin：扩展函数
来源：http://hz.52xcode.cn/gtstcvvqbd.html

fun String.exclaim() = this + "!"
来源：http://hz.cheryme.top/gtwavmkrdw.html

[T10] Kotlin：默认参数
来源：http://hz.andypj.xyz/gttcvydlds.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cdnleiting.top/gtjuiqhlac.html

[T11] Kotlin：协程
来源：http://hz.nwbrower.top/gtlvffmzxo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jlsjyb.cn/gtvmhkhqkc.html

[T12] Kotlin：解构声明
来源：http://hz.svipenyu.cn/gtszipyqwc.html

val (a, b) = Pair(1, 2)
来源：http://hz.316326.xyz/gtsvylwssw.html

[T13] Kotlin：只读 Map
来源：http://hz.hongshengwenyu.top/gtqbacfzhr.html

val m = mapOf("a" to 1)
来源：http://hz.jiagoushi.top/gtfjkhkwmg.html

[T14] Kotlin：循环
来源：http://hz.meibo888.top/gtrewxpovd.html

for (i in 1..10) println(i)
来源：http://hz.kuanghao11.cn/gtnyfzyfns.html

[T15] Kotlin：接口
来源：http://hz.chenzaomai.com/gtyzsvigou.html

interface Shape { fun area(): Double }
来源：http://hz.chenjidiqi.icu/gtphzgevyc.html

[T16] Swift：Hello World
来源：http://hz.iojbl.cn/gtrpcrrwtl.html

print("Hello")
来源：http://hz.sxryk.cn/gtrbtzwesy.html

[T17] Swift：变量与常量
来源：http://hz.jinghuilouyu.cn/gtpxqkjvgl.html

var a = 1;  let b = 2
来源：http://hz.bjfxy.top/gtpeysxhbl.html

[T18] Swift：字符串插值
来源：http://hz.zhengqikj.top/gthheygwzo.html

"值: \(b)"
来源：http://hz.birdmap.top/gtrzzqxhsb.html

[T19] Swift：可选绑定
来源：http://hz.wangdashe.top/gtexledfdt.html

if let n = opt { print(n) }
来源：http://hz.fengsongda.top/gtahdxtldz.html

[T20] Swift：数组操作
来源：http://hz.svipenyu.cn/gtzntodrtx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhaomingkeji.xyz/gtpacyhzrz.html

[T21] Swift：遍历
来源：http://hz.316326.xyz/gtreqopfzs.html

for x in a { print(x) }
来源：http://hz.yueranfly.top/gtbnohzddh.html

[T22] Swift：字典
来源：http://hz.jianghu66.top/gttltcguxi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxinkj.top/gtfnvnrvqh.html

[T23] Swift：函数
来源：http://hz.andypj.xyz/gtnpwkqfgk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cucudq.cn/gtnjgtyvzf.html

[T24] Swift：闭包
来源：http://hz.jqgfzy.top/gtkdswnhmi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xuetiantiany.cn/gtjeunsvhv.html

[T25] Swift：结构体
来源：http://hz.zhijiandao.cn/gtwmsuxtvf.html

struct P { var x: Int }
来源：http://hz.iojbl.cn/gttsufemnq.html

[T26] Swift：类与重写
来源：http://hz.shangyingyoupin.top/gtgyuubgcy.html

class A: Base { override func f() {} }
来源：http://hz.zhixingplan.top/gtklpytqqs.html

[T27] Swift：错误处理
来源：http://hz.yangfankeji.com/gtrzrqjxqh.html

do { try f() } catch { print(error) }
来源：http://hz.shuidangran.top/gtrwnnoivw.html

[T28] Swift：枚举
来源：http://hz.mhx1999.top/gtyzbhbooe.html

enum Color { case red, green }
来源：http://hz.zhixingplan.top/gtrvylbkgo.html

[T29] Swift：guard 提前返回
来源：http://hz.daria6918.cn/gtnvlsnudm.html

guard let x = opt else { return }
来源：http://hz.yvedp.cn/gtxhtzcroc.html

[T30] Swift：协议
来源：http://hz.wangdashe.top/gtdscexwdk.html

protocol Shape { func area() -> Double }
来源：http://hz.haohaochexian.top/gttuxofpdu.html

[T31] Lua：Hello World
来源：http://hz.jinghuilouyu.cn/gtwvlqgibs.html

print("Hello")
来源：http://hz.jiagoushi.top/gtlhbplbns.html

[T32] Lua：局部变量
来源：http://hz.zdqjudy.top/gtinbnkrsy.html

local a = 1
来源：http://hz.shanyushiyangkeji.top/gtqvqssqvy.html

[T33] Lua：表（数组）
来源：http://hz.smart0.xyz/gtycmiorpk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cdnleiting.top/gtjexvbjok.html

[T34] Lua：遍历表
来源：http://hz.yangfankeji.com/gtgysbfvng.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.svipenyu.cn/gticvmeuxn.html

[T35] Lua：字典表
来源：http://hz.daxiang520.top/gtrfstaaaa.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhijiandao.cn/gtyyuuoeyn.html

[T36] Lua：函数
来源：http://hz.snrcjt.cn/gtxgotoygl.html

function add(a, b) return a + b end
来源：http://hz.shzxlz.cn/gtbnjciknx.html

[T37] Lua：字符串拼接
来源：http://hz.shuidangran.top/gtefqtegvh.html

"a" .. "b"
来源：http://hz.jinghuilouyu.cn/gtldezbcut.html

[T38] Lua：条件
来源：http://hz.svipenyu.cn/gtipzspjyq.html

if x > 0 then print("正") end
来源：http://hz.dashuyun.cn/gtjvzheefj.html

[T39] Lua：模式匹配
来源：http://hz.yj20258888.top/gtsoygixjp.html

string.find(s, "%d+")
来源：http://hz.hnxiangtu.top/gtsnghkqei.html

[T40] Lua：元表
来源：http://hz.ydzc1.top/gtgswwszwf.html

setmetatable({}, { __index = base })
来源：http://hz.meibo888.top/gtakradmtg.html

[T41] Perl：Hello World
来源：http://hz.jianghu66.top/gtnfrjkbpx.html

print "Hello\n";
来源：http://hz.vqdsnc.cn/gtttyljrqj.html

[T42] Perl：变量类型
来源：http://hz.zhijiandao.cn/gtkohyvsjx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhijiandao.cn/gtibadzzmi.html

[T43] Perl：字符串插值
来源：http://hz.smart0.xyz/gtmdqickju.html

"值: $a"
来源：http://hz.yangfankeji.com/gtnplxrcar.html

[T44] Perl：条件
来源：http://hz.guannengcc.top/gtvjpwsnrc.html

if ($a > 0) { print "正"; }
来源：http://hz.yj202588.top/gteeovgmoh.html

[T45] Perl：数组遍历
来源：http://hz.aizwys.cn/gtimrmmpeh.html

for my $x (@arr) { print $x; }
来源：http://hz.yangfankeji.com/gteywwoiwp.html

[T46] Perl：哈希操作
来源：http://hz.cdnleiting.top/gtjuymbsch.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.aibaodan.cn/gtdwscgrec.html

[T47] Perl：正则捕获
来源：http://hz.yj20258888.top/gtonalsuvz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yangfankeji.com/gtxdmhyqvl.html

[T48] Perl：正则替换
来源：http://hz.jinqigfzy.top/gtfxuywjke.html

$s =~ s/old/new/g;
来源：http://hz.gzhubu.top/gtqsbhlibk.html

[T49] Perl：函数
来源：http://hz.shanyushiyangkeji.top/gtivwmquxw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.kuanghao11.cn/gthpxhtumz.html

[T50] Perl：逐行读文件
来源：http://hz.cheryme.top/gtfvhrjwru.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhaomingkeji.xyz/gtpxceuzgh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yongpay.top/gtvcrgtvtm.html

[T51] Scala：Hello World
来源：http://hz.svipenyu.cn/gtrmffazqt.html

println("Hello")
来源：http://hz.xuetiantiany.cn/gtiyfukbyq.html

[T52] Scala：变量
来源：http://hz.smart0.xyz/gtbyqlmner.html

val a = 1;  var b = 2
来源：http://hz.sxryk.cn/gttvjumsoo.html

[T53] Scala：字符串插值
来源：http://hz.feifeiyinyue.top/gtxahrsfjg.html

s"值: $b"
来源：http://hz.jyoumei.cn/gtfzaurrei.html

[T54] Scala：集合映射
来源：http://hz.jqgufenzy.top/gtfzbevihr.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zdqjudy.top/gtysgzqtuy.html

[T55] Scala：集合过滤
来源：http://hz.ehwqpu.com/gtialdagke.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.nwbrower.top/gtnrqpgnhf.html

[T56] Scala：样例类
来源：http://hz.fzhhl.top/gtzcpourxo.html

case class User(name: String, age: Int)
来源：http://hz.9152youxi.cn/gtgmsuqmvp.html

[T57] Scala：模式匹配
来源：http://hz.9152youxi.cn/gtbznimika.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xinyue.icu/gtmhqasjsj.html

[T58] Scala：函数定义
来源：http://hz.hnxiangtu.top/gtrviadgpu.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xylfe.cn/gtzqvrtsnu.html

[T59] Scala：循环
来源：http://hz.dianchejie.cn/gtkpyugpvm.html

for (i <- 1 to 10) println(i)
来源：http://hz.mhx1999.top/gtmwwxyaeg.html

[T60] Scala：折叠
来源：http://hz.gaohongyu789.top/gtcgcjwnpu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yanxiufei.cn/gtbaokykwy.html

================================================================================
来源：http://hz.yangfankeji.com/gtjmuocwgv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj202588.top/gtybwtfpmw.html

================================================================================
来源：http://hz.haohaochexian.top/gtgwwgplbk.html

[U01] Py：创建虚拟环境
来源：http://hz.tianlin.xyz/gtwapledmq.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhaomingkeji.xyz/gtulrkbfdx.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenlongwang.top/gtayimfiyr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenlongwang.top/gticlqshhu.html

[U03] Py：加载 .env 配置
来源：http://hz.jyoumei.cn/gtcpwlqsrd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xziqi.cn/gtncziogow.html

[U04] Py：变量调试打印
来源：http://hz.shuidangran.top/gtkkbflvvs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.iojbl.cn/gtowbrnwsw.html

[U05] Py：列表去重且保序
来源：http://hz.gaohongyu789.top/gtavnqpsdt.html

list(dict.fromkeys(arr))
来源：http://hz.zhiwuduotai.top/gtgrwbfeqc.html

[U06] Py：合并两个字典
来源：http://hz.zycfv.cn/gtnkfktjun.html

{**a, **b}
来源：http://hz.kuanghao11.cn/gtybdwyimq.html

[U07] Py：反转字典键值
来源：http://hz.ydzc1.top/gtbwnlxpgs.html

{v: k for k, v in d.items()}
来源：http://hz.iojbl.cn/gthnafqvsb.html

[U08] Py：展平二维列表
来源：http://hz.cheryme.top/gtpqsaflsf.html

[y for x in nested for y in x]
来源：http://hz.jqgufenzy.top/gtwhvrdlhi.html

[U09] Py：字典取最大值的键
来源：http://hz.xylfe.cn/gtzwevdsfv.html

max(d, key=d.get)
来源：http://hz.tianlin.xyz/gtewgsctis.html

[U10] Py：按值排序字典
来源：http://hz.daria6918.cn/gtpyohsbeh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hywenlv.cn/gtfylbgjhy.html

[U11] Py：生成器表达式
来源：http://hz.yuanzhike.top/gtljzfiufn.html

(x * 2 for x in arr)
来源：http://hz.sxryk.cn/gtpqrjasux.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.iojbl.cn/gtvmyecarr.html

Counter(arr).most_common(3)
来源：http://hz.jqgufenzy.top/gtdfidbdyb.html

[U13] Py：固定长度队列
来源：http://hz.zhaomingkeji.xyz/gtnpnqepdy.html

deque(maxlen=10)
来源：http://hz.cqqwz.cn/gtsbhjxtlt.html

[U14] Py：分组收集到列表
来源：http://hz.sysykeji.top/gtjnohmtpl.html

defaultdict(list)
来源：http://hz.0kj1m.cn/gthgccfzxp.html

[U15] Py：高精度计时
来源：http://hz.wangdashe.top/gtmcjrjpco.html

t = time.perf_counter()
来源：http://hz.guannengcc.top/gtkfhwpraz.html

[U16] Py：命令行参数解析
来源：http://hz.fengsongda.top/gtihqtktyi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.svipenyu.cn/gtqcqhbacv.html

[U17] Py：初始化日志
来源：http://hz.gzhubu.top/gtvfqrcggo.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xingfuxueyuan.xyz/gtkokmrurs.html

[U18] Py：预编译正则
来源：http://hz.sufxvd.cn/gtezwxemqi.html

pat = re.compile(r"\d+")
来源：http://hz.sufxvd.cn/gtlxlgouvd.html

[U19] Py：正则替换带回调
来源：http://hz.9152youxi.cn/gtwgkovcmo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sysykeji.top/gtepabufih.html

[U20] Py：缓存函数结果
来源：http://hz.xuetiantiany.cn/gtomdzksnj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ywan-chungtsiang.top/gtwkqaccdx.html

[U21] Py：自定义上下文管理器
来源：http://hz.dashuyun.cn/gtkouphltm.html

@contextlib.contextmanager
来源：http://hz.andypj.xyz/gtrdmimdbf.html

[U22] Py：矩阵转置
来源：http://hz.xuetiantiany.cn/gtkocbwxmp.html

list(zip(*m))
来源：http://hz.zhijiandao.cn/gtfvyhoghe.html

[U23] Py：分块读取大文件
来源：http://hz.daxiang520.top/gtbhmhcrvs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shzxlz.cn/gtybgrnbqx.html

[U24] Py：路径操作
来源：http://hz.aibaodan.cn/gtqlctwhsf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cheryme.top/gtarkfxsrk.html

[U25] Py：CSV 按字典读
来源：http://hz.feifeiyinyue.top/gtvsgxvndk.html

csv.DictReader(f)
来源：http://hz.feifeiyinyue.top/gtmtmpfxfh.html

[U26] Py：并发下载
来源：http://hz.jlsjyb.cn/gtfvdzcpfc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.316326.xyz/gtnmzxcycm.html

[U27] Py：异步 HTTP
来源：http://hz.xziqi.cn/gtsesdwsob.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hysaishi.cn/gtwlaszwqa.html

[U28] Py：类型别名
来源：http://hz.chenzaomai.com/gtamqwotpf.html

UserId = int
来源：http://hz.zhiwuduotai.top/gtqhyfmnxw.html

[U29] Py：属性校验
来源：http://hz.sysykeji.top/gtyooenfrb.html

@property 与 @x.setter 配合
来源：http://hz.hywenlv.cn/gtasnhejkh.html

[U30] Py：数据类
来源：http://hz.zhixingplan.top/gttlloiusw.html

@dataclass(slots=True)
来源：http://hz.yj20258888.top/gtlrcrslib.html

[U31] Py：单测
来源：http://hz.hnxiangtu.top/gtwdckshtw.html

python -m pytest -q
来源：http://hz.ydjk.org.cn/gtpqqdnfnw.html

[U32] Py：代码格式化
来源：http://hz.ehwqpu.com/gtrabzmjay.html

ruff format . && ruff check --fix .
来源：http://hz.chenzaomai.com/gtlsfxzdea.html

[U33] Py：打包发布
来源：http://hz.zhengqikj.top/gtwvswhzwe.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ivvv.top/gtdpshfuip.html

[U34] Py：判断编码
来源：http://hz.wangshuangyany.cn/gtqcpuhjun.html

chardet.detect(raw)
来源：http://hz.pengpengdd.cyou/gtzliymbgm.html

[U35] Py：发送邮件
来源：http://hz.jyoumei.cn/gtwodzwhxz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yuanzhike.top/gtusfkgygp.html

[U36] Py：定时任务
来源：http://hz.tanke756.top/gtxapcjuai.html

schedule.every(10).minutes.do(job)
来源：http://hz.snrcjt.cn/gtdouxcxte.html

[U37] Py：读写 Excel
来源：http://hz.jlsjyb.cn/gtorxmobwl.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shuidangran.top/gtfejdcthr.html

[U38] Py：获取脚本所在目录
来源：http://hz.sufxvd.cn/gtnoglptpo.html

Path(__file__).resolve().parent
来源：http://hz.aibaodan.cn/gtcnsietld.html

[U39] Py：判断是否在交互环境
来源：http://hz.fzhhl.top/gtikhlyyev.html

sys.stdout.isatty()
来源：http://hz.jinyuanbaomall.cn/gtrzwqxnbd.html

[U40] Py：打印到标准错误
来源：http://hz.hongshengwenyu.top/gtxydzalsy.html

print("err", file=sys.stderr)
来源：http://hz.jinqigufen.top/gtcbdkrxxw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ivvv.top/gtaixgrxtm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.meibo888.top/gtpshdpgut.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gzhubu.top/gtkmqthaeb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ybcxt.top/gtbhbtmofo.html

[U43] PHP：声明命名空间
来源：http://hz.tianlin.xyz/gthgosaozy.html

namespace App\Http;
来源：http://hz.xinyue.icu/gtxjgnbxda.html

[U44] PHP：开启严格类型
来源：http://hz.ywan-chungtsiang.top/gtpkkevisa.html

declare(strict_types=1);
来源：http://hz.svipenyu.cn/gtqkngwqlx.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ydjk.org.cn/gtmowlbknl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ybcxt.top/gtqrhiudid.html

[U46] PHP：可空类型
来源：http://hz.ydzc1.top/gtglxgigcz.html

?string $name = null
来源：http://hz.yj20258888.top/gtlpjreeom.html

[U47] PHP：联合类型
来源：http://hz.quarkkingdee.top/gtbsyxyymm.html

int|string $id
来源：http://hz.9152youxi.cn/gtemkmjbuf.html

[U48] PHP：纯枚举
来源：http://hz.ivvv.top/gterkpigsi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shzxlz.cn/gttbcfwmta.html

[U49] PHP：只读属性
来源：http://hz.tian-w.cn/gtgrdvckvn.html

public readonly string $name
来源：http://hz.yonumen.top/gtaknwnrcm.html

[U50] PHP：构造器属性提升
来源：http://hz.redwolf501.top/gtovvebknt.html

public function __construct(private int $id) {}
来源：http://hz.guowangkeji.top/gtkqjziowy.html

[U51] PHP：数组解构
来源：http://hz.zycfv.cn/gtmekucdww.html

[$a, $b] = $arr;
来源：http://hz.nanxinkj.top/gtyazvaqib.html

[U52] PHP：箭头函数
来源：http://hz.aibaodan.cn/gtnssgfano.html

$double = fn($x) => $x * 2;
来源：http://hz.ybcxt.top/gtdgfnicxe.html

[U53] PHP：空合并运算符
来源：http://hz.gzhubu.top/gtojgyzcwl.html

$v = $a ?? $b ?? "default";
来源：http://hz.zdqjudy.top/gtkbuwqjxu.html

[U54] PHP：空安全调用
来源：http://hz.sxryk.cn/gtzlmzssye.html

$obj?->method()
来源：http://hz.yonumen.top/gtuxrnzmhq.html

[U55] PHP：match 表达式
来源：http://hz.zhoulong.xyz/gttokaxlic.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jlsjyb.cn/gtoyilkask.html

[U56] PHP：命名参数
来源：http://hz.0kj1m.cn/gtsfcpllfw.html

f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gteewojpzm.html

[U57] PHP：字符串插值
来源：http://hz.hywenlv.cn/gtltispnfy.html

"值: {$a}"
来源：http://hz.sweek.top/gtwoysayiy.html

[U58] PHP：数组三件套
来源：http://hz.wangdashe.top/gtipfckujx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.tian-w.cn/gtnsxsnfaz.html

[U59] PHP：自定义排序
来源：http://hz.cucudq.cn/gtfjtlpecc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.kuanghao11.cn/gtqcdmfvxl.html

[U60] PHP：JSON 编解码
来源：http://hz.cdnleiting.top/gtrnhryqxc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hysaishi.cn/gtalsgamvu.html

[U61] PHP：正则
来源：http://hz.yanxiufei.cn/gtmbbvkrxn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangtech.top/gtbkysfcrd.html

[U62] PHP：日期对象
来源：http://hz.gogol.net.cn/gtyeiykthr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sweek.top/gtegcjlqgm.html

[U63] PHP：文件读写
来源：http://hz.ppjwa.cn/gtsdgxczbi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yongpay.top/gtyizedvou.html

[U64] PHP：目录遍历
来源：http://hz.hnxiangtu.top/gtdgcvbckz.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.shuidangran.top/gtwgsrgjff.html

[U65] PHP：会话
来源：http://hz.mhx1999.top/gtkiinrphj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yanxiufei.cn/gtxkojlchn.html

[U66] PHP：设置 Cookie
来源：http://hz.smart0.xyz/gtkziqlqvw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.sweek.top/gtjbxldgzl.html

[U67] PHP：处理文件上传
来源：http://hz.wangshuangyany.cn/gtopfuvbzh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.sufxvd.cn/gtoulinlrm.html

[U68] PHP：PDO 连接
来源：http://hz.aibaodan.cn/gtemagywcp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.wangshuangyany.cn/gtdpqdsmyb.html

[U69] PHP：PDO 预处理
来源：http://hz.guannengcc.top/gtsoyhjfbs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xingfuxueyuan.xyz/gtajilgxfo.html

[U70] PHP：PDO 事务
来源：http://hz.gotoacloud.top/gtxgbqprfp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.wangshuangyany.cn/gtpymydgno.html

[U71] PHP：抛出异常
来源：http://hz.cdnleiting.top/gtaxluycjo.html

throw new RuntimeException("失败", 500);
来源：http://hz.nanxuanxn.top/gtcqmevjbb.html

[U72] PHP：写错误日志
来源：http://hz.zhoulong.xyz/gtcsusreln.html

error_log("失败: " . $e->getMessage());
来源：http://hz.chenzaomai.com/gtpzhddbsi.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhaomingkeji.xyz/gtkaopewrp.html

parse_ini_file("config.ini", true)
来源：http://hz.ivvv.top/gtwwuuqmyx.html

[U74] PHP：读取环境变量
来源：http://hz.ppjwa.cn/gtgmeyeimj.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhaomingkeji.xyz/gtxobudnrv.html

[U75] PHP：依赖注入
来源：http://hz.yuxming.cn/gtwnzxyrmd.html

composer require psr/container
来源：http://hz.aibaodan.cn/gtmqjmzugr.html

[U76] PHP：简单路由
来源：http://hz.tanke756.top/gtqzhiqvct.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhengqikj.top/gtkdwzmbhu.html

[U77] PHP：模板渲染
来源：http://hz.sxryk.cn/gteafmmhfq.html

composer require twig/twig
来源：http://hz.mhx1999.top/gtvecedkrx.html

[U78] PHP：单元测试
来源：http://hz.kuanghao11.cn/gtaatloojb.html

composer require --dev phpunit/phpunit
来源：http://hz.pengpengdd.cyou/gtwqpyjcdg.html

[U79] PHP：静态分析
来源：http://hz.chenjidiqi.icu/gtrdedewcc.html

composer require --dev phpstan/phpstan
来源：http://hz.kuanghao11.cn/gtloyoxpre.html

[U80] PHP：代码规范修复
来源：http://hz.sysykeji.top/gtswwwlhay.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.smart0.xyz/gtazgfserh.html


<!-- 参考信息 -->