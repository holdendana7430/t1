代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.0kj1m.cn/gtzlevlhsr.html

[S57] C++：编译期常量
来源：http://hz.shuidangran.top/gtttrrbwfo.html

constexpr int N = 10;
来源：http://hz.hysaishi.cn/gtdaljpasp.html

[S58] C++：命名空间
来源：http://hz.snrcjt.cn/gtdznnxalg.html

namespace ns { int f() { return 1; } }
来源：http://hz.9152youxi.cn/gtnjifcpyz.html

[S59] C++：静态断言
来源：http://hz.fzhhl.top/gtxoobffes.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tanke756.top/gtoycwbizd.html

[S60] C++：遍历并删除元素
来源：http://hz.fengsongda.top/gtmkjgntil.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenjidiqi.icu/gtbbjltmkj.html

================================================================================
来源：http://hz.nanxinkj.top/gtgmfeakdk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sysykeji.top/gtitmymvim.html

================================================================================
来源：http://hz.yj202588.top/gtlwstolpp.html

[T01] Kotlin：Hello World
来源：http://hz.mhx1999.top/gteaymtmvb.html

println("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtwrboftml.html

[T02] Kotlin：变量
来源：http://hz.tianlin.xyz/gtrohydzlz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangdashe.top/gtkcfooctx.html

[T03] Kotlin：字符串模板
来源：http://hz.hfpthk.cn/gtnxstqqdl.html

"值: $b"
来源：http://hz.tianlin.xyz/gtasznzzto.html

[T04] Kotlin：空安全
来源：http://hz.ehwqpu.com/gtgtokhxfe.html

val n: String? = null;  n?.length
来源：http://hz.feifeiyinyue.top/gtxkutgmxx.html

[T05] Kotlin：when 表达式
来源：http://hz.bjfxy.top/gtsgclivnt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhaomingkeji.xyz/gtkjtakguq.html

[T06] Kotlin：集合映射
来源：http://hz.hfpthk.cn/gtzqmnntkr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gotoacloud.top/gttgkpijme.html

[T07] Kotlin：集合过滤
来源：http://hz.iojbl.cn/gtxiqxdafe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.birdmap.top/gtwszomhzn.html

[T08] Kotlin：数据类
来源：http://hz.gogol.net.cn/gtrrehfgov.html

data class User(val name: String, val age: Int)
来源：http://hz.jinghuilouyu.cn/gtopkbapja.html

[T09] Kotlin：扩展函数
来源：http://hz.redwolf501.top/gtzvisaqwn.html

fun String.exclaim() = this + "!"
来源：http://hz.hnxiangtu.top/gtueqgxizv.html

[T10] Kotlin：默认参数
来源：http://hz.redwolf501.top/gtteqviyey.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.vqdsnc.cn/gtmxnebmfn.html

[T11] Kotlin：协程
来源：http://hz.guannengcc.top/gtmoaaikrm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daxiang520.top/gtmgpbxohx.html

[T12] Kotlin：解构声明
来源：http://hz.chenlongwang.top/gtuwhktfqy.html

val (a, b) = Pair(1, 2)
来源：http://hz.kuanghao11.cn/gtezqfzhci.html

[T13] Kotlin：只读 Map
来源：http://hz.9152youxi.cn/gtdwhybogb.html

val m = mapOf("a" to 1)
来源：http://hz.daxiang520.top/gtlrgyrmzc.html

[T14] Kotlin：循环
来源：http://hz.hfpthk.cn/gtukkbijto.html

for (i in 1..10) println(i)
来源：http://hz.cheryme.top/gtiiriyaav.html

[T15] Kotlin：接口
来源：http://hz.wangshuangyany.cn/gthjmiylro.html

interface Shape { fun area(): Double }
来源：http://hz.yueranfly.top/gtvkffokpk.html

[T16] Swift：Hello World
来源：http://hz.cheryme.top/gtposjfxph.html

print("Hello")
来源：http://hz.jinqigfzy.top/gtagovafid.html

[T17] Swift：变量与常量
来源：http://hz.gaohongyu789.top/gtnslzotho.html

var a = 1;  let b = 2
来源：http://hz.birdmap.top/gtzwlrmunl.html

[T18] Swift：字符串插值
来源：http://hz.tianlin.xyz/gtpjieynhb.html

"值: \(b)"
来源：http://hz.fengsongda.top/gtvhphaskp.html

[T19] Swift：可选绑定
来源：http://hz.yanxiufei.cn/gtdujfhhdi.html

if let n = opt { print(n) }
来源：http://hz.snrcjt.cn/gtafaizjqi.html

[T20] Swift：数组操作
来源：http://hz.zhaomingkeji.xyz/gtyormgavh.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shzxlz.cn/gtxqakelsn.html

[T21] Swift：遍历
来源：http://hz.iojbl.cn/gtmnaowaag.html

for x in a { print(x) }
来源：http://hz.zhoulong.xyz/gttmrllwnm.html

[T22] Swift：字典
来源：http://hz.jyoumei.cn/gtwlfozuru.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jianghu66.top/gtqantuouy.html

[T23] Swift：函数
来源：http://hz.havefunace.top/gtfaqgpeeg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tianlin.xyz/gttdzyjbos.html

[T24] Swift：闭包
来源：http://hz.jinqigfzy.top/gtcsmdhgkk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jqgfzy.top/gtmgbelgst.html

[T25] Swift：结构体
来源：http://hz.yuanzhike.top/gtqthmpcfx.html

struct P { var x: Int }
来源：http://hz.zycfv.cn/gthmzjxzvx.html

[T26] Swift：类与重写
来源：http://hz.xinyue.icu/gtgxbilsvq.html

class A: Base { override func f() {} }
来源：http://hz.zhaomingkeji.xyz/gtpltlysax.html

[T27] Swift：错误处理
来源：http://hz.jiagoushi.top/gtznogcpvt.html

do { try f() } catch { print(error) }
来源：http://hz.gotoacloud.top/gtleomynhc.html

[T28] Swift：枚举
来源：http://hz.52xcode.cn/gtdqchdtlj.html

enum Color { case red, green }
来源：http://hz.vqdsnc.cn/gtekelhoao.html

[T29] Swift：guard 提前返回
来源：http://hz.shuidangran.top/gtcudymadl.html

guard let x = opt else { return }
来源：http://hz.yangfankeji.com/gtdmcikzhi.html

[T30] Swift：协议
来源：http://hz.hywenlv.cn/gtcpxzrehj.html

protocol Shape { func area() -> Double }
来源：http://hz.sufxvd.cn/gtvxwuyqbh.html

[T31] Lua：Hello World
来源：http://hz.aibaodan.cn/gtdubztegs.html

print("Hello")
来源：http://hz.sweek.top/gtdqbzberd.html

[T32] Lua：局部变量
来源：http://hz.ywan-chungtsiang.top/gtjdnsiohj.html

local a = 1
来源：http://hz.tian-w.cn/gtcngpllfx.html

[T33] Lua：表（数组）
来源：http://hz.daxiang520.top/gtyetanmom.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xinyue.icu/gtpodnqzux.html

[T34] Lua：遍历表
来源：http://hz.ehwqpu.com/gtylbgeicd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sxryk.cn/gtirkfodhd.html

[T35] Lua：字典表
来源：http://hz.cdnleiting.top/gtqvrvffnu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj20258888.top/gttshmisxo.html

[T36] Lua：函数
来源：http://hz.9152youxi.cn/gtttwfwseo.html

function add(a, b) return a + b end
来源：http://hz.sysykeji.top/gthqlqxart.html

[T37] Lua：字符串拼接
来源：http://hz.mhx1999.top/gticsgffnd.html

"a" .. "b"
来源：http://hz.pycfn.com/gtnfpmhfmk.html

[T38] Lua：条件
来源：http://hz.zhengqikj.top/gtclpmqcup.html

if x > 0 then print("正") end
来源：http://hz.birdmap.top/gtzpjeteog.html

[T39] Lua：模式匹配
来源：http://hz.zhongyouzk.top/gtneaczhmp.html

string.find(s, "%d+")
来源：http://hz.yvedp.cn/gtsrebbvhw.html

[T40] Lua：元表
来源：http://hz.xuanzx.com/gtzgrlwwai.html

setmetatable({}, { __index = base })
来源：http://hz.hfpthk.cn/gtrqemzmdm.html

[T41] Perl：Hello World
来源：http://hz.tanke756.top/gtndldmluv.html

print "Hello\n";
来源：http://hz.dashuyun.cn/gttxlpctbi.html

[T42] Perl：变量类型
来源：http://hz.pycfn.com/gtqigchvic.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yuanzhike.top/gtjkhrkovf.html

[T43] Perl：字符串插值
来源：http://hz.snrcjt.cn/gtuipjkqir.html

"值: $a"
来源：http://hz.meibo888.top/gtsfzwyjgl.html

[T44] Perl：条件
来源：http://hz.jinqigfzy.top/gtvqwqfmok.html

if ($a > 0) { print "正"; }
来源：http://hz.feifeiyinyue.top/gtmbbzpoyc.html

[T45] Perl：数组遍历
来源：http://hz.zhongyouzk.top/gteschsydv.html

for my $x (@arr) { print $x; }
来源：http://hz.hnqzz.top/gtphrlwipc.html

[T46] Perl：哈希操作
来源：http://hz.0kj1m.cn/gtbtgupehd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.feifeiyinyue.top/gtaiwqgkee.html

[T47] Perl：正则捕获
来源：http://hz.ydzc1.top/gtgwmvnllr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sysykeji.top/gtonyrglua.html

[T48] Perl：正则替换
来源：http://hz.cheryme.top/gtvpfrspwo.html

$s =~ s/old/new/g;
来源：http://hz.hysaishi.cn/gtvgloxjev.html

[T49] Perl：函数
来源：http://hz.vqdsnc.cn/gtnsdvwfqp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhijiandao.cn/gtfskqgvts.html

[T50] Perl：逐行读文件
来源：http://hz.yonumen.top/gtluvvdeyw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenjidiqi.icu/gtawzgsmjo.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.redwolf501.top/gtdrsdhllu.html

[T51] Scala：Hello World
来源：http://hz.yj20258888.top/gtwvegjtnt.html

println("Hello")
来源：http://hz.zhijiandao.cn/gthwjnlxwu.html

[T52] Scala：变量
来源：http://hz.tian-w.cn/gtboxyqtjl.html

val a = 1;  var b = 2
来源：http://hz.yongpay.top/gtazcfxurx.html

[T53] Scala：字符串插值
来源：http://hz.kuanghao11.cn/gtzptbcfsk.html

s"值: $b"
来源：http://hz.zdqjudy.top/gtmsoevvlf.html

[T54] Scala：集合映射
来源：http://hz.tanke756.top/gtsznpegni.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhijiandao.cn/gtgvyfropf.html

[T55] Scala：集合过滤
来源：http://hz.chenjidiqi.icu/gtpwxqbyeg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.316326.xyz/gtmxljalbg.html

[T56] Scala：样例类
来源：http://hz.dianchejie.cn/gtvyegoftd.html

case class User(name: String, age: Int)
来源：http://hz.jinqigfzy.top/gtnmmrdjun.html

[T57] Scala：模式匹配
来源：http://hz.guannengcc.top/gtqcavpfyz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.havefunace.top/gtucjfatwx.html

[T58] Scala：函数定义
来源：http://hz.shzxlz.cn/gtmqkdkqdn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.gaohongyu789.top/gtjlefabsv.html

[T59] Scala：循环
来源：http://hz.jinqigufen.top/gtqfxjbqvc.html

for (i <- 1 to 10) println(i)
来源：http://hz.pengpengdd.cyou/gtemfhndpg.html

[T60] Scala：折叠
来源：http://hz.wangshuangyany.cn/gtcxgsddrk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.guannengcc.top/gtaoevxhom.html

================================================================================
来源：http://hz.shuidangran.top/gtndupdruu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.dashuyun.cn/gtgbfwfluj.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtdwytlepp.html

[U01] Py：创建虚拟环境
来源：http://hz.chenzaomai.com/gtjhjhfjwv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.redwolf501.top/gtwnivtopb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shuidangran.top/gtdsaacifi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.haohaochexian.top/gtfyekybzf.html

[U03] Py：加载 .env 配置
来源：http://hz.jlsjyb.cn/gtdlpdogyu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.chenzaomai.com/gtxbhkslhg.html

[U04] Py：变量调试打印
来源：http://hz.redwolf501.top/gtrxcxybhh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zdqjudy.top/gtsxngvwqv.html

[U05] Py：列表去重且保序
来源：http://hz.zhijiandao.cn/gtzaqzufhv.html

list(dict.fromkeys(arr))
来源：http://hz.hysaishi.cn/gtzactynfg.html

[U06] Py：合并两个字典
来源：http://hz.316326.xyz/gtyccbrsjj.html

{**a, **b}
来源：http://hz.gzhubu.top/gtspynsesy.html

[U07] Py：反转字典键值
来源：http://hz.fzhhl.top/gtkbyglqlv.html

{v: k for k, v in d.items()}
来源：http://hz.xuetiantiany.cn/gthbbyzswg.html

[U08] Py：展平二维列表
来源：http://hz.jqgfzy.top/gtmmhdienw.html

[y for x in nested for y in x]
来源：http://hz.9152youxi.cn/gtvtusooua.html

[U09] Py：字典取最大值的键
来源：http://hz.nanxuanxn.top/gterxfontp.html

max(d, key=d.get)
来源：http://hz.9152youxi.cn/gtrwyzgjsp.html

[U10] Py：按值排序字典
来源：http://hz.gogol.net.cn/gtjdrdnmip.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.svipenyu.cn/gtjqiamdwf.html

[U11] Py：生成器表达式
来源：http://hz.ppjwa.cn/gtonqfmnaw.html

(x * 2 for x in arr)
来源：http://hz.shanyushiyangkeji.top/gttuxirfgf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gzhubu.top/gtnakyfsxy.html

Counter(arr).most_common(3)
来源：http://hz.zhaomingkeji.xyz/gtegzkogad.html

[U13] Py：固定长度队列
来源：http://hz.cashguo.top/gtietvkazq.html

deque(maxlen=10)
来源：http://hz.dashuyun.cn/gtrnhsthns.html

[U14] Py：分组收集到列表
来源：http://hz.andypj.xyz/gtujrljlen.html

defaultdict(list)
来源：http://hz.zhengqikj.top/gtiiwgrmly.html

[U15] Py：高精度计时
来源：http://hz.smart0.xyz/gtpzyjcaxi.html

t = time.perf_counter()
来源：http://hz.hysaishi.cn/gtnghfpdoi.html

[U16] Py：命令行参数解析
来源：http://hz.cucudq.cn/gtvtpcdjst.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.shanyushiyangkeji.top/gtdtfkauxj.html

[U17] Py：初始化日志
来源：http://hz.smart0.xyz/gtndobrxja.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.aizwys.cn/gtkalkwplg.html

[U18] Py：预编译正则
来源：http://hz.bjfxy.top/gtwkzkelpz.html

pat = re.compile(r"\d+")
来源：http://hz.cheryme.top/gtxgntwmat.html

[U19] Py：正则替换带回调
来源：http://hz.chenzaomai.com/gttvqblqar.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.dashuyun.cn/gtfzyrrdxc.html

[U20] Py：缓存函数结果
来源：http://hz.pycfn.com/gtwnhviyke.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinqigfzy.top/gtjxocvlww.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhijiandao.cn/gtjufidbnt.html

@contextlib.contextmanager
来源：http://hz.snrcjt.cn/gtlwokmsfe.html

[U22] Py：矩阵转置
来源：http://hz.wangdashe.top/gtzlnkijgb.html

list(zip(*m))
来源：http://hz.ppjwa.cn/gtriuzbkmc.html

[U23] Py：分块读取大文件
来源：http://hz.havefunace.top/gtzcnjmjub.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jqgufenzy.top/gtuvgdntvf.html

[U24] Py：路径操作
来源：http://hz.yanxiufei.cn/gtgmsrxhoc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shuidangran.top/gtmcrecoir.html

[U25] Py：CSV 按字典读
来源：http://hz.fengsongda.top/gtxocfsurh.html

csv.DictReader(f)
来源：http://hz.tian-w.cn/gtgnwperha.html

[U26] Py：并发下载
来源：http://hz.ehwqpu.com/gtptujbzbi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.9152youxi.cn/gtihmeooxa.html

[U27] Py：异步 HTTP
来源：http://hz.dianchejie.cn/gtjklohtom.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ehwqpu.com/gtpctdjapo.html

[U28] Py：类型别名
来源：http://hz.cashguo.top/gtstnvczff.html

UserId = int
来源：http://hz.tanke756.top/gtdoqxthoa.html

[U29] Py：属性校验
来源：http://hz.smart0.xyz/gtmwdykeaq.html

@property 与 @x.setter 配合
来源：http://hz.hnxiangtu.top/gtkhfkdnnj.html

[U30] Py：数据类
来源：http://hz.jiagoushi.top/gtbnbwsriq.html

@dataclass(slots=True)
来源：http://hz.cucudq.cn/gtcawklyex.html

[U31] Py：单测
来源：http://hz.hammf.cn/gtrexqaxpp.html

python -m pytest -q
来源：http://hz.haohaochexian.top/gtsbzbdwgi.html

[U32] Py：代码格式化
来源：http://hz.hammf.cn/gtjakddpun.html

ruff format . && ruff check --fix .
来源：http://hz.cqqwz.cn/gtzqavreeg.html

[U33] Py：打包发布
来源：http://hz.andypj.xyz/gttffiancx.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.fengsongda.top/gtprqhtowi.html

[U34] Py：判断编码
来源：http://hz.cashguo.top/gttvibdkfo.html

chardet.detect(raw)
来源：http://hz.daxiang520.top/gtpilktjww.html

[U35] Py：发送邮件
来源：http://hz.zdqjudy.top/gtpjtdsgmi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hammf.cn/gtgmxmlfjo.html

[U36] Py：定时任务
来源：http://hz.vqdsnc.cn/gtbmraesxg.html

schedule.every(10).minutes.do(job)
来源：http://hz.tanke756.top/gtlxjgfphm.html

[U37] Py：读写 Excel
来源：http://hz.andypj.xyz/gtwpkprszf.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ydjk.org.cn/gtvlcyxoaz.html

[U38] Py：获取脚本所在目录
来源：http://hz.xylfe.cn/gtjocpkrhh.html

Path(__file__).resolve().parent
来源：http://hz.kuanghao11.cn/gtrrtxgtri.html

[U39] Py：判断是否在交互环境
来源：http://hz.ehwqpu.com/gthwvbdabn.html

sys.stdout.isatty()
来源：http://hz.birdmap.top/gtweqqoudb.html

[U40] Py：打印到标准错误
来源：http://hz.ppjwa.cn/gtzpgywckm.html

print("err", file=sys.stderr)
来源：http://hz.ydzc1.top/gtzbfoksol.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shanyushiyangtech.top/gtqqgxhuaf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cheryme.top/gttpblmkdi.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sxryk.cn/gtatuxnyah.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.c1oappe.top/gtlsjjpaxh.html

[U43] PHP：声明命名空间
来源：http://hz.quarkkingdee.top/gtbmrpizml.html

namespace App\Http;
来源：http://hz.gaohongyu789.top/gtkrhdnbui.html

[U44] PHP：开启严格类型
来源：http://hz.aibaodan.cn/gthufpjlyl.html

declare(strict_types=1);
来源：http://hz.zhijiandao.cn/gtbqbpminz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shzxlz.cn/gtbyhglwdi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtmrymrklp.html

[U46] PHP：可空类型
来源：http://hz.chenlongwang.top/gtdewtnrsu.html

?string $name = null
来源：http://hz.ehwqpu.com/gtoorcdbtz.html

[U47] PHP：联合类型
来源：http://hz.cdnleiting.top/gtuycungvr.html

int|string $id
来源：http://hz.chenlongwang.top/gtlvaowfsq.html

[U48] PHP：纯枚举
来源：http://hz.ydzc1.top/gthrmxyclb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhaomingkeji.xyz/gtqeqwmfdf.html

[U49] PHP：只读属性
来源：http://hz.cashguo.top/gtecmbnrfo.html

public readonly string $name
来源：http://hz.jqgufenzy.top/gtejgobebz.html

[U50] PHP：构造器属性提升
来源：http://hz.zhijiandao.cn/gtphbauoek.html

public function __construct(private int $id) {}
来源：http://hz.cucudq.cn/gtmzunxgro.html

[U51] PHP：数组解构
来源：http://hz.daria6918.cn/gtgizfosnr.html

[$a, $b] = $arr;
来源：http://hz.yueranfly.top/gtmgelgtcx.html

[U52] PHP：箭头函数
来源：http://hz.cucudq.cn/gtctggotoc.html

$double = fn($x) => $x * 2;
来源：http://hz.nwbrower.top/gtyktaiyjf.html

[U53] PHP：空合并运算符
来源：http://hz.feifeiyinyue.top/gtjsufdgtj.html

$v = $a ?? $b ?? "default";
来源：http://hz.quarkkingdee.top/gtoepwxkbv.html

[U54] PHP：空安全调用
来源：http://hz.svipenyu.cn/gtrrwpqgqq.html

$obj?->method()
来源：http://hz.shanyushiyangkeji.top/gtthixieuw.html

[U55] PHP：match 表达式
来源：http://hz.gaohongyu789.top/gthisohjjw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sxryk.cn/gtatxlcdsm.html

[U56] PHP：命名参数
来源：http://hz.jlsjyb.cn/gtartnwscb.html

f(a: 1, b: 2)
来源：http://hz.hfpthk.cn/gtvcdfbrcr.html

[U57] PHP：字符串插值
来源：http://hz.cdnleiting.top/gtwuxugfpy.html

"值: {$a}"
来源：http://hz.chenlongwang.top/gtecyqxziz.html

[U58] PHP：数组三件套
来源：http://hz.hammf.cn/gtbyscauax.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.feifeiyinyue.top/gtqjnaqgue.html

[U59] PHP：自定义排序
来源：http://hz.xylfe.cn/gtjnpqexbg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fengsongda.top/gtenlmyipv.html

[U60] PHP：JSON 编解码
来源：http://hz.yuxming.cn/gtyrypoyny.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhiwuduotai.top/gtzrovwjfw.html

[U61] PHP：正则
来源：http://hz.yueranfly.top/gtdrjbmxjr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cheryme.top/gthteqjurd.html

[U62] PHP：日期对象
来源：http://hz.kuanghao11.cn/gtmxmgfubl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.shzxlz.cn/gtgckivjdl.html

[U63] PHP：文件读写
来源：http://hz.9152youxi.cn/gtlmobodsb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xuetiantiany.cn/gthevexqff.html

[U64] PHP：目录遍历
来源：http://hz.svipenyu.cn/gtgzrdqspo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ydzc1.top/gtnhqkjfta.html

[U65] PHP：会话
来源：http://hz.kuanghao11.cn/gtkkyigkto.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.cheryme.top/gttnidnyjr.html

[U66] PHP：设置 Cookie
来源：http://hz.pycfn.com/gtdvdemnpj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yonumen.top/gtddghedus.html

[U67] PHP：处理文件上传
来源：http://hz.nanxinkj.top/gtowlqhkhc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.wangshuangyany.cn/gtapwjjwjz.html

[U68] PHP：PDO 连接
来源：http://hz.52xcode.cn/gtcxqniige.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhengqikj.top/gtgywthhqs.html

[U69] PHP：PDO 预处理
来源：http://hz.jinyuanbaomall.cn/gtzhchzgvw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.chenjidiqi.icu/gtfygexdom.html

[U70] PHP：PDO 事务
来源：http://hz.xuetiantiany.cn/gtmrlckxhv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.316326.xyz/gtzvcwqdit.html

[U71] PHP：抛出异常
来源：http://hz.zhijiandao.cn/gtbftlfsvm.html

throw new RuntimeException("失败", 500);
来源：http://hz.dianchejie.cn/gtljllsqwi.html

[U72] PHP：写错误日志
来源：http://hz.fzhhl.top/gtqnhobdgp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hfpthk.cn/gtaosgkyne.html

[U73] PHP：读取 ini 配置
来源：http://hz.shzxlz.cn/gtmpsluntd.html

parse_ini_file("config.ini", true)
来源：http://hz.ppjwa.cn/gthajzfvly.html

[U74] PHP：读取环境变量
来源：http://hz.yangfankeji.com/gtiggisbai.html

getenv("APP_ENV") ?: "production"
来源：http://hz.chenjidiqi.icu/gtzjncstku.html

[U75] PHP：依赖注入
来源：http://hz.snrcjt.cn/gthyhhswlz.html

composer require psr/container
来源：http://hz.tian-w.cn/gtixxqbxzr.html

[U76] PHP：简单路由
来源：http://hz.yueranfly.top/gtcfqvvrcn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.quarkkingdee.top/gtqyaydlgd.html

[U77] PHP：模板渲染
来源：http://hz.cqqwz.cn/gtfsaogbos.html

composer require twig/twig
来源：http://hz.9152youxi.cn/gtkimmtuyf.html

[U78] PHP：单元测试
来源：http://hz.yanxiufei.cn/gtrufdbvkl.html

composer require --dev phpunit/phpunit
来源：http://hz.zhaomingkeji.xyz/gtmsxwmobl.html

[U79] PHP：静态分析
来源：http://hz.yj20258888.top/gtnpkilyhb.html

composer require --dev phpstan/phpstan
来源：http://hz.zhoulong.xyz/gtomqjejfe.html

[U80] PHP：代码规范修复
来源：http://hz.jyoumei.cn/gttipvegkd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.aibaodan.cn/gtgzyopwaw.html

[U81] JS：初始化项目
来源：http://hz.havefunace.top/gtnhxxyljd.html

npm init -y;  npm i express
来源：http://hz.hammf.cn/gtyrfmodoz.html

[U82] JS：package.json 脚本
来源：http://hz.wangdashe.top/gtmujmlqfg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.redwolf501.top/gtxolvfoyo.html


<!-- 参考信息 -->