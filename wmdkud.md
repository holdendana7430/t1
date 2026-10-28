代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gotoacloud.top/gtabqbhygf.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangkeji.top/gtmrauodko.html

static_cast<double>(a) / b
来源：http://hz.shuidangran.top/gtnipkjtac.html

[S52] C++：const 与 noexcept
来源：http://hz.zycfv.cn/gtxistmkhq.html

int size() const noexcept { return n_; }
来源：http://hz.shanyushiyangtech.top/gtekrgymlu.html

[S53] C++：移动语义
来源：http://hz.dianchejie.cn/gtfxzqroir.html

std::vector<int> w = std::move(v);
来源：http://hz.xingfuxueyuan.xyz/gtqvdfvwyf.html

[S54] C++：异常处理
来源：http://hz.jyoumei.cn/gtlvyyesyl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shuidangran.top/gtvgykjsre.html

[S55] C++：结构化绑定
来源：http://hz.ydzc1.top/gtozzyvzhb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhongyouzk.top/gtftkwihrv.html

[S56] C++：optional
来源：http://hz.tianlin.xyz/gtngnzwpdn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.daxiang520.top/gtpazfzscr.html

[S57] C++：编译期常量
来源：http://hz.jinqigufen.top/gtcemzvvby.html

constexpr int N = 10;
来源：http://hz.smart0.xyz/gtkoitastq.html

[S58] C++：命名空间
来源：http://hz.nanxinkj.top/gtvifwuywe.html

namespace ns { int f() { return 1; } }
来源：http://hz.sxryk.cn/gtexgncfvn.html

[S59] C++：静态断言
来源：http://hz.yj20258888.top/gtpkorxwnz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hammf.cn/gtjkpucylh.html

[S60] C++：遍历并删除元素
来源：http://hz.havefunace.top/gtgxqoniha.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhongyouzk.top/gtbcpirgvb.html

================================================================================
来源：http://hz.xinyue.icu/gthmxctuwi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.c1oappe.top/gtjwylvblz.html

================================================================================
来源：http://hz.vqdsnc.cn/gtnpocdkak.html

[T01] Kotlin：Hello World
来源：http://hz.jqgufenzy.top/gtjenwqerp.html

println("Hello")
来源：http://hz.yj20258.top/gtsmyxjeve.html

[T02] Kotlin：变量
来源：http://hz.aizwys.cn/gtzscntwno.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.meibo888.top/gtdcaqtxke.html

[T03] Kotlin：字符串模板
来源：http://hz.jinqigufen.top/gtjarloziz.html

"值: $b"
来源：http://hz.sufxvd.cn/gtoieyctkz.html

[T04] Kotlin：空安全
来源：http://hz.pengpengdd.cyou/gtffxixsaa.html

val n: String? = null;  n?.length
来源：http://hz.chenlongwang.top/gtaqpccnqz.html

[T05] Kotlin：when 表达式
来源：http://hz.zhongyouzk.top/gtzatasbao.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xinyue.icu/gtxutmaaln.html

[T06] Kotlin：集合映射
来源：http://hz.jlsjyb.cn/gtjaoqzbwb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydjk.org.cn/gttoqimokm.html

[T07] Kotlin：集合过滤
来源：http://hz.yonumen.top/gtztqyysxu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xylfe.cn/gthjctwtvl.html

[T08] Kotlin：数据类
来源：http://hz.hongshengwenyu.top/gtehdrfquc.html

data class User(val name: String, val age: Int)
来源：http://hz.redwolf501.top/gtsiidyhff.html

[T09] Kotlin：扩展函数
来源：http://hz.sufxvd.cn/gtsyfryzmx.html

fun String.exclaim() = this + "!"
来源：http://hz.jqgufenzy.top/gtexrtkecx.html

[T10] Kotlin：默认参数
来源：http://hz.hnqzz.top/gtpqgwrwzg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hammf.cn/gtmaplifko.html

[T11] Kotlin：协程
来源：http://hz.hywenlv.cn/gtgodhsqsq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xingfuxueyuan.xyz/gtkyozdaof.html

[T12] Kotlin：解构声明
来源：http://hz.jinyuanbaomall.cn/gthytkyods.html

val (a, b) = Pair(1, 2)
来源：http://hz.birdmap.top/gtwklxrcwi.html

[T13] Kotlin：只读 Map
来源：http://hz.zhaomingkeji.xyz/gtbqlxekmx.html

val m = mapOf("a" to 1)
来源：http://hz.shangyingyoupin.top/gtaicceekd.html

[T14] Kotlin：循环
来源：http://hz.wangdashe.top/gtmedayjrq.html

for (i in 1..10) println(i)
来源：http://hz.svipenyu.cn/gttoszrmcj.html

[T15] Kotlin：接口
来源：http://hz.hysaishi.cn/gtfshnrdwk.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gtdvndfgdd.html

[T16] Swift：Hello World
来源：http://hz.ywan-chungtsiang.top/gtowvjejsa.html

print("Hello")
来源：http://hz.jinqigfzy.top/gtnuocrzlb.html

[T17] Swift：变量与常量
来源：http://hz.zycfv.cn/gtdgluxfnu.html

var a = 1;  let b = 2
来源：http://hz.haohaochexian.top/gtqlxlnkyg.html

[T18] Swift：字符串插值
来源：http://hz.nwbrower.top/gtvnlyajhi.html

"值: \(b)"
来源：http://hz.quarkkingdee.top/gtiacvmnfy.html

[T19] Swift：可选绑定
来源：http://hz.tianlin.xyz/gtmizokraj.html

if let n = opt { print(n) }
来源：http://hz.ydjk.org.cn/gtqsluzsfg.html

[T20] Swift：数组操作
来源：http://hz.cqqwz.cn/gtfoegicjx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhongyouzk.top/gtsctioixu.html

[T21] Swift：遍历
来源：http://hz.aizwys.cn/gtzahcckyy.html

for x in a { print(x) }
来源：http://hz.yuanzhike.top/gtacpbeoxq.html

[T22] Swift：字典
来源：http://hz.quarkkingdee.top/gtjcfwumxz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sufxvd.cn/gtmyjjemwx.html

[T23] Swift：函数
来源：http://hz.nwbrower.top/gtxklnwkru.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.birdmap.top/gtuicsikkk.html

[T24] Swift：闭包
来源：http://hz.zycfv.cn/gtasyffjvb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shangyingyoupin.top/gtunchjwtt.html

[T25] Swift：结构体
来源：http://hz.shuidangran.top/gtigkebqwp.html

struct P { var x: Int }
来源：http://hz.jinqigfzy.top/gtjkzyghgg.html

[T26] Swift：类与重写
来源：http://hz.kuanghao11.cn/gtwzuctehi.html

class A: Base { override func f() {} }
来源：http://hz.sxryk.cn/gtjnfwwmjk.html

[T27] Swift：错误处理
来源：http://hz.hnqzz.top/gtfzzoausa.html

do { try f() } catch { print(error) }
来源：http://hz.yuxming.cn/gtihnvnzag.html

[T28] Swift：枚举
来源：http://hz.hfpthk.cn/gtjiqimkyv.html

enum Color { case red, green }
来源：http://hz.iojbl.cn/gtjcppbwwg.html

[T29] Swift：guard 提前返回
来源：http://hz.nwbrower.top/gtnywflaoe.html

guard let x = opt else { return }
来源：http://hz.pycfn.com/gtsrdpreyl.html

[T30] Swift：协议
来源：http://hz.tian-w.cn/gthisfgojh.html

protocol Shape { func area() -> Double }
来源：http://hz.snrcjt.cn/gtwoalhhff.html

[T31] Lua：Hello World
来源：http://hz.fengsongda.top/gtzvgsdfjr.html

print("Hello")
来源：http://hz.9152youxi.cn/gtudcorcuf.html

[T32] Lua：局部变量
来源：http://hz.tianlin.xyz/gtcmcqglpk.html

local a = 1
来源：http://hz.316326.xyz/gtvmwurotm.html

[T33] Lua：表（数组）
来源：http://hz.wangdashe.top/gtendwqrwk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yuxming.cn/gtvpbvgloy.html

[T34] Lua：遍历表
来源：http://hz.52xcode.cn/gtmeiltgir.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinghuilouyu.cn/gttgsdwagh.html

[T35] Lua：字典表
来源：http://hz.xziqi.cn/gtzapwkvpo.html

local d = { a = 1 };  d.b = 2
来源：http://hz.pengpengdd.cyou/gtzftraiel.html

[T36] Lua：函数
来源：http://hz.c1oappe.top/gtlldeygje.html

function add(a, b) return a + b end
来源：http://hz.yj20258.top/gtzzquiqfk.html

[T37] Lua：字符串拼接
来源：http://hz.yueranfly.top/gtdwhfexcw.html

"a" .. "b"
来源：http://hz.52xcode.cn/gtluvnuxxr.html

[T38] Lua：条件
来源：http://hz.shuidangran.top/gtpolzsmbi.html

if x > 0 then print("正") end
来源：http://hz.zycfv.cn/gtolfjrgpl.html

[T39] Lua：模式匹配
来源：http://hz.zhoulong.xyz/gtmxhekurl.html

string.find(s, "%d+")
来源：http://hz.birdmap.top/gtgqtmnhqf.html

[T40] Lua：元表
来源：http://hz.fzhhl.top/gtlvyffnwd.html

setmetatable({}, { __index = base })
来源：http://hz.havefunace.top/gtgggqvbvl.html

[T41] Perl：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtjlzlcchz.html

print "Hello\n";
来源：http://hz.zhoulong.xyz/gtaufhxkbr.html

[T42] Perl：变量类型
来源：http://hz.gzhubu.top/gtxvqvxchn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.havefunace.top/gtzqtvphxd.html

[T43] Perl：字符串插值
来源：http://hz.cdnleiting.top/gteczwuefu.html

"值: $a"
来源：http://hz.yueranfly.top/gtlpouybqt.html

[T44] Perl：条件
来源：http://hz.nanxinkj.top/gtajfpmykr.html

if ($a > 0) { print "正"; }
来源：http://hz.guannengcc.top/gtauynrwzq.html

[T45] Perl：数组遍历
来源：http://hz.redwolf501.top/gtjssxenda.html

for my $x (@arr) { print $x; }
来源：http://hz.jlsjyb.cn/gtyyixkadk.html

[T46] Perl：哈希操作
来源：http://hz.jyoumei.cn/gtpbpjhsjm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xziqi.cn/gtkzlhxjfy.html

[T47] Perl：正则捕获
来源：http://hz.iojbl.cn/gtujeqpzvz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cdnleiting.top/gttroyvddh.html

[T48] Perl：正则替换
来源：http://hz.xuetiantiany.cn/gtsbulpglt.html

$s =~ s/old/new/g;
来源：http://hz.shangyingyoupin.top/gtzeiliofu.html

[T49] Perl：函数
来源：http://hz.quarkkingdee.top/gtztgrgvkr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tianlin.xyz/gtdhuepqsf.html

[T50] Perl：逐行读文件
来源：http://hz.chenjidiqi.icu/gtogjdgbtx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.meibo888.top/gtvlcsmtsh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.snrcjt.cn/gtjqgsaoub.html

[T51] Scala：Hello World
来源：http://hz.yangfankeji.com/gtbcdecnkl.html

println("Hello")
来源：http://hz.hywenlv.cn/gtjrxvstze.html

[T52] Scala：变量
来源：http://hz.yuanzhike.top/gtokwykohn.html

val a = 1;  var b = 2
来源：http://hz.hfpthk.cn/gtxrvigyas.html

[T53] Scala：字符串插值
来源：http://hz.ybcxt.top/gtequyzgwe.html

s"值: $b"
来源：http://hz.zhijiandao.cn/gtvxkhlden.html

[T54] Scala：集合映射
来源：http://hz.yueranfly.top/gtfvzuhgbg.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.c1oappe.top/gtpixgfkii.html

[T55] Scala：集合过滤
来源：http://hz.zhaomingkeji.xyz/gtfjofsspb.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sysykeji.top/gtkcrcbjtn.html

[T56] Scala：样例类
来源：http://hz.quarkkingdee.top/gtiuqnqpts.html

case class User(name: String, age: Int)
来源：http://hz.zhaomingkeji.xyz/gtfnaodmvu.html

[T57] Scala：模式匹配
来源：http://hz.gzhubu.top/gtpjpvuisd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.fzhhl.top/gtzgthoggy.html

[T58] Scala：函数定义
来源：http://hz.jinqigfzy.top/gtuxnocwdq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yuxming.cn/gtskifiqyi.html

[T59] Scala：循环
来源：http://hz.tanke756.top/gtjpalczzs.html

for (i <- 1 to 10) println(i)
来源：http://hz.dianchejie.cn/gtutcdpbrg.html

[T60] Scala：折叠
来源：http://hz.xingfuxueyuan.xyz/gtydznfbrg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yangfankeji.com/gtrvwfhqmy.html

================================================================================
来源：http://hz.meibo888.top/gtkskbrqyn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tian-w.cn/gtmcbzvwcz.html

================================================================================
来源：http://hz.zhixingplan.top/gtqlwpraqo.html

[U01] Py：创建虚拟环境
来源：http://hz.cqqwz.cn/gtpndlzwow.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.guowangkeji.top/gtixnpwkqp.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cdnleiting.top/gtvalzljnv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shanyushiyangtech.top/gtjciunswy.html

[U03] Py：加载 .env 配置
来源：http://hz.zhoulong.xyz/gtxpvftqwz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.snrcjt.cn/gtnijgqyqt.html

[U04] Py：变量调试打印
来源：http://hz.dianchejie.cn/gtjsmomijr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gotoacloud.top/gtjsqerzat.html

[U05] Py：列表去重且保序
来源：http://hz.zhijiandao.cn/gtyolwqbwn.html

list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gtoqwwllqb.html

[U06] Py：合并两个字典
来源：http://hz.chenzaomai.com/gtuqidtknw.html

{**a, **b}
来源：http://hz.cdnleiting.top/gterpucrze.html

[U07] Py：反转字典键值
来源：http://hz.ivvv.top/gtsltxzada.html

{v: k for k, v in d.items()}
来源：http://hz.zhongyouzk.top/gthnslyflb.html

[U08] Py：展平二维列表
来源：http://hz.jiagoushi.top/gtwlrdxctm.html

[y for x in nested for y in x]
来源：http://hz.gogol.net.cn/gtfjdvudmy.html

[U09] Py：字典取最大值的键
来源：http://hz.chenlongwang.top/gtvsbkzqij.html

max(d, key=d.get)
来源：http://hz.havefunace.top/gtptfscoex.html

[U10] Py：按值排序字典
来源：http://hz.xinyue.icu/gtoebijbkl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinyuanbaomall.cn/gtfzrkxycj.html

[U11] Py：生成器表达式
来源：http://hz.jiagoushi.top/gtnmwrxdeo.html

(x * 2 for x in arr)
来源：http://hz.tianlin.xyz/gtfkqnhtvi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.nanxinkj.top/gtafugmlth.html

Counter(arr).most_common(3)
来源：http://hz.bjfxy.top/gtmeuwseof.html

[U13] Py：固定长度队列
来源：http://hz.tian-w.cn/gtkmkkfkfp.html

deque(maxlen=10)
来源：http://hz.cashguo.top/gtugktaryz.html

[U14] Py：分组收集到列表
来源：http://hz.smart0.xyz/gtgpdnapco.html

defaultdict(list)
来源：http://hz.zhoulong.xyz/gtgozwlkmo.html

[U15] Py：高精度计时
来源：http://hz.xuetiantiany.cn/gtrzyoxkzm.html

t = time.perf_counter()
来源：http://hz.shangyingyoupin.top/gtyjeyfgot.html

[U16] Py：命令行参数解析
来源：http://hz.jinqigufen.top/gtvmrytoom.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yanxiufei.cn/gtrcgucgev.html

[U17] Py：初始化日志
来源：http://hz.svipenyu.cn/gthydxfcvw.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shanyushiyangkeji.top/gtzensbyhf.html

[U18] Py：预编译正则
来源：http://hz.daxiang520.top/gtxavmxbqi.html

pat = re.compile(r"\d+")
来源：http://hz.zhaomingkeji.xyz/gtltgkcwkn.html

[U19] Py：正则替换带回调
来源：http://hz.jyoumei.cn/gtwugxpyth.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hywenlv.cn/gtublfnzao.html

[U20] Py：缓存函数结果
来源：http://hz.cheryme.top/gtmaugkmhm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhoulong.xyz/gtnkojjfeb.html

[U21] Py：自定义上下文管理器
来源：http://hz.yanxiufei.cn/gttowznvvb.html

@contextlib.contextmanager
来源：http://hz.havefunace.top/gtvgiogsvn.html

[U22] Py：矩阵转置
来源：http://hz.haohaochexian.top/gtimwaiejf.html

list(zip(*m))
来源：http://hz.aizwys.cn/gtljcqpncd.html

[U23] Py：分块读取大文件
来源：http://hz.cucudq.cn/gtuvjumeuc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.chenlongwang.top/gtbnueozzi.html

[U24] Py：路径操作
来源：http://hz.gzhubu.top/gtqbscodqy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinqigfzy.top/gtmzfpvltl.html

[U25] Py：CSV 按字典读
来源：http://hz.yangfankeji.com/gtqxpvmynq.html

csv.DictReader(f)
来源：http://hz.ydzc1.top/gtqhyoqfwl.html

[U26] Py：并发下载
来源：http://hz.jinyuanbaomall.cn/gtxicoeata.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.9152youxi.cn/gtjjfaawhj.html

[U27] Py：异步 HTTP
来源：http://hz.vqdsnc.cn/gtvpfgrhzi.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.daxiang520.top/gtocdgivtu.html

[U28] Py：类型别名
来源：http://hz.dianchejie.cn/gtrdsfnmeo.html

UserId = int
来源：http://hz.daria6918.cn/gtxycofgoa.html

[U29] Py：属性校验
来源：http://hz.zhijiandao.cn/gtieqbhoem.html

@property 与 @x.setter 配合
来源：http://hz.0kj1m.cn/gtggvledar.html

[U30] Py：数据类
来源：http://hz.zycfv.cn/gthszoodlk.html

@dataclass(slots=True)
来源：http://hz.daria6918.cn/gtfsvixvqz.html

[U31] Py：单测
来源：http://hz.cucudq.cn/gtbjzqandk.html

python -m pytest -q
来源：http://hz.redwolf501.top/gtdpteplge.html

[U32] Py：代码格式化
来源：http://hz.cucudq.cn/gtitehftzu.html

ruff format . && ruff check --fix .
来源：http://hz.cheryme.top/gtoldplgyj.html

[U33] Py：打包发布
来源：http://hz.zhiwuduotai.top/gtmrosfiet.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hywenlv.cn/gtaiglmpkf.html

[U34] Py：判断编码
来源：http://hz.cashguo.top/gtcowfwvuf.html

chardet.detect(raw)
来源：http://hz.gotoacloud.top/gtubsfezgv.html

[U35] Py：发送邮件
来源：http://hz.hongshengwenyu.top/gtxjchgmxf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hongshengwenyu.top/gtmkhzfrah.html

[U36] Py：定时任务
来源：http://hz.zhengqikj.top/gtsavrmaby.html

schedule.every(10).minutes.do(job)
来源：http://hz.andypj.xyz/gtgfezewzw.html

[U37] Py：读写 Excel
来源：http://hz.redwolf501.top/gtbfvpiwvv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yuanzhike.top/gtfewznxab.html

[U38] Py：获取脚本所在目录
来源：http://hz.nanxinkj.top/gtfnkyzvyc.html

Path(__file__).resolve().parent
来源：http://hz.aibaodan.cn/gtzlaoyzew.html

[U39] Py：判断是否在交互环境
来源：http://hz.ehwqpu.com/gtloakfrir.html

sys.stdout.isatty()
来源：http://hz.xinyue.icu/gtybwocqzb.html

[U40] Py：打印到标准错误
来源：http://hz.haohaochexian.top/gtgenkkxii.html

print("err", file=sys.stderr)
来源：http://hz.fengsongda.top/gtdbcovblx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.wangdashe.top/gtdcbqzglx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hammf.cn/gteeypnwfm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shanyushiyangkeji.top/gthymmxlka.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jyoumei.cn/gtmpjsezfl.html

[U43] PHP：声明命名空间
来源：http://hz.yanxiufei.cn/gtuhpaknyv.html

namespace App\Http;
来源：http://hz.hfpthk.cn/gtetzudfvs.html

[U44] PHP：开启严格类型
来源：http://hz.zycfv.cn/gtfcgfbsol.html

declare(strict_types=1);
来源：http://hz.daria6918.cn/gtzthplmzb.html

[U45] PHP：类型声明与返回类型
来源：http://hz.pycfn.com/gtxowsfzew.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhoulong.xyz/gthxccjydu.html

[U46] PHP：可空类型
来源：http://hz.hnqzz.top/gtnibosxie.html

?string $name = null
来源：http://hz.hywenlv.cn/gtnueqjife.html

[U47] PHP：联合类型
来源：http://hz.yj20258888.top/gtldnwieaj.html

int|string $id
来源：http://hz.ppjwa.cn/gtshjaooqu.html

[U48] PHP：纯枚举
来源：http://hz.hammf.cn/gtldptkuhc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.wangdashe.top/gtatttgozt.html

[U49] PHP：只读属性
来源：http://hz.ehwqpu.com/gtsbbicegb.html

public readonly string $name
来源：http://hz.chenlongwang.top/gtynwmrlua.html

[U50] PHP：构造器属性提升
来源：http://hz.fengsongda.top/gtgcrngfnj.html

public function __construct(private int $id) {}
来源：http://hz.zhongyouzk.top/gtuyhvavxk.html

[U51] PHP：数组解构
来源：http://hz.yonumen.top/gtjyufnwut.html

[$a, $b] = $arr;
来源：http://hz.jinqigfzy.top/gtbafmvywj.html

[U52] PHP：箭头函数
来源：http://hz.snrcjt.cn/gtpezmaiuu.html

$double = fn($x) => $x * 2;
来源：http://hz.zycfv.cn/gtabnhjcdw.html

[U53] PHP：空合并运算符
来源：http://hz.meibo888.top/gtvkswdffj.html

$v = $a ?? $b ?? "default";
来源：http://hz.sufxvd.cn/gtvdekfbyr.html

[U54] PHP：空安全调用
来源：http://hz.yanxiufei.cn/gtmlwmoqtw.html

$obj?->method()
来源：http://hz.zycfv.cn/gthufalnxd.html

[U55] PHP：match 表达式
来源：http://hz.yueranfly.top/gtdvyeetrg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hammf.cn/gtsjrpiowf.html

[U56] PHP：命名参数
来源：http://hz.hnqzz.top/gtelneyqiq.html

f(a: 1, b: 2)
来源：http://hz.ehwqpu.com/gtovuzmtze.html

[U57] PHP：字符串插值
来源：http://hz.nanxinkj.top/gtsvqhmbxp.html

"值: {$a}"
来源：http://hz.cheryme.top/gtmjuxmfjk.html

[U58] PHP：数组三件套
来源：http://hz.dianchejie.cn/gtrriiguwt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.haohaochexian.top/gtzmvsjlhk.html

[U59] PHP：自定义排序
来源：http://hz.havefunace.top/gtwpwoyagi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.meibo888.top/gtplpdzjko.html

[U60] PHP：JSON 编解码
来源：http://hz.shanyushiyangtech.top/gtpnvshmxa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.tanke756.top/gtypcwtxig.html

[U61] PHP：正则
来源：http://hz.xuanzx.com/gtqmbekefq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.havefunace.top/gtwmwhqtsr.html

[U62] PHP：日期对象
来源：http://hz.ppjwa.cn/gtmxizbqaf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.xylfe.cn/gtwfbpagab.html

[U63] PHP：文件读写
来源：http://hz.jyoumei.cn/gtdjyvqxlc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jqgufenzy.top/gtxjnsaivg.html

[U64] PHP：目录遍历
来源：http://hz.hysaishi.cn/gteewdmakm.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.nwbrower.top/gtrhyndbtb.html

[U65] PHP：会话
来源：http://hz.zhengqikj.top/gtfgtnopjc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.chenlongwang.top/gtyljedbiy.html

[U66] PHP：设置 Cookie
来源：http://hz.yj20258888.top/gtwjhndrtp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.guowangkeji.top/gtrfxqdtbv.html

[U67] PHP：处理文件上传
来源：http://hz.yanxiufei.cn/gthcutpmln.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.iojbl.cn/gtlhhgbjew.html

[U68] PHP：PDO 连接
来源：http://hz.9152youxi.cn/gtkwrgtbja.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hongshengwenyu.top/gthtdzoeww.html

[U69] PHP：PDO 预处理
来源：http://hz.dashuyun.cn/gtlngnsdfr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jqgfzy.top/gtwtyhkrbp.html

[U70] PHP：PDO 事务
来源：http://hz.pycfn.com/gtqdgarhsa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.9152youxi.cn/gtdpwqqxhm.html

[U71] PHP：抛出异常
来源：http://hz.yj202588.top/gtjxsvlpei.html

throw new RuntimeException("失败", 500);
来源：http://hz.andypj.xyz/gtzkortcpw.html

[U72] PHP：写错误日志
来源：http://hz.cashguo.top/gtylhkgtkw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cdnleiting.top/gtlsqxawiw.html

[U73] PHP：读取 ini 配置
来源：http://hz.hammf.cn/gttbxdlays.html

parse_ini_file("config.ini", true)
来源：http://hz.yj202588.top/gtjeyjthqo.html

[U74] PHP：读取环境变量
来源：http://hz.yueranfly.top/gtmcwmpswm.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zdqjudy.top/gtahudvkxj.html

[U75] PHP：依赖注入
来源：http://hz.smart0.xyz/gtgbjzskpn.html

composer require psr/container
来源：http://hz.jinqigfzy.top/gtlzcxutid.html

[U76] PHP：简单路由
来源：http://hz.c1oappe.top/gtzpvpxxqh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yanxiufei.cn/gtbjhhkmgd.html


<!-- 参考信息 -->