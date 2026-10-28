代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.birdmap.top/gthyaqgwsx.html

[S57] C++：编译期常量
来源：http://hz.bjfxy.top/gtfpsblsqp.html

constexpr int N = 10;
来源：http://hz.sufxvd.cn/gthkjaquzm.html

[S58] C++：命名空间
来源：http://hz.ydjk.org.cn/gtahvhkvqq.html

namespace ns { int f() { return 1; } }
来源：http://hz.yonumen.top/gtiyhgxfgt.html

[S59] C++：静态断言
来源：http://hz.vqdsnc.cn/gtxzvwgrmk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shangyingyoupin.top/gtmowytfyb.html

[S60] C++：遍历并删除元素
来源：http://hz.vqdsnc.cn/gtkqinojnp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dianchejie.cn/gtawgjqcdb.html

================================================================================
来源：http://hz.cucudq.cn/gtzffikqnu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydjk.org.cn/gtapsnnqiu.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtvzczsjkh.html

[T01] Kotlin：Hello World
来源：http://hz.chenlongwang.top/gtwalrfjfe.html

println("Hello")
来源：http://hz.jlsjyb.cn/gtvroqrvmj.html

[T02] Kotlin：变量
来源：http://hz.cheryme.top/gtyxpwxupf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.dashuyun.cn/gtiipdxvui.html

[T03] Kotlin：字符串模板
来源：http://hz.birdmap.top/gtxbciczds.html

"值: $b"
来源：http://hz.jlsjyb.cn/gtgfttlxvp.html

[T04] Kotlin：空安全
来源：http://hz.guannengcc.top/gtfvkkxnhv.html

val n: String? = null;  n?.length
来源：http://hz.yj202588.top/gtjmalmgjw.html

[T05] Kotlin：when 表达式
来源：http://hz.wangshuangyany.cn/gtgsklbtrm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigufen.top/gtiumtbgua.html

[T06] Kotlin：集合映射
来源：http://hz.wangdashe.top/gtzucbjqye.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.52xcode.cn/gtsoemohkk.html

[T07] Kotlin：集合过滤
来源：http://hz.zycfv.cn/gtvndvmeiq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuxming.cn/gtddkkplyi.html

[T08] Kotlin：数据类
来源：http://hz.ybcxt.top/gthshizuio.html

data class User(val name: String, val age: Int)
来源：http://hz.tanke756.top/gtdpdsputy.html

[T09] Kotlin：扩展函数
来源：http://hz.mhx1999.top/gthswjaeye.html

fun String.exclaim() = this + "!"
来源：http://hz.yvedp.cn/gtnkshnmyz.html

[T10] Kotlin：默认参数
来源：http://hz.cucudq.cn/gtaolkgjlq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aizwys.cn/gtnvykyffs.html

[T11] Kotlin：协程
来源：http://hz.ivvv.top/gtpfshrfkc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.redwolf501.top/gtkzqfpfem.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtyiioqjfo.html

val (a, b) = Pair(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtjqgvnmta.html

[T13] Kotlin：只读 Map
来源：http://hz.hywenlv.cn/gttryqnvai.html

val m = mapOf("a" to 1)
来源：http://hz.xinyue.icu/gtsqsiicqm.html

[T14] Kotlin：循环
来源：http://hz.gogol.net.cn/gtjcljkhay.html

for (i in 1..10) println(i)
来源：http://hz.aizwys.cn/gthbvmydgi.html

[T15] Kotlin：接口
来源：http://hz.yanxiufei.cn/gtwtisgoun.html

interface Shape { fun area(): Double }
来源：http://hz.yvedp.cn/gtjigaupzl.html

[T16] Swift：Hello World
来源：http://hz.9152youxi.cn/gtenbbstsr.html

print("Hello")
来源：http://hz.jinqigfzy.top/gtuyfghsvg.html

[T17] Swift：变量与常量
来源：http://hz.wangshuangyany.cn/gtfmkbixea.html

var a = 1;  let b = 2
来源：http://hz.gzhubu.top/gtttckpoaj.html

[T18] Swift：字符串插值
来源：http://hz.guowangkeji.top/gtwrolcusb.html

"值: \(b)"
来源：http://hz.daxiang520.top/gtplkloevu.html

[T19] Swift：可选绑定
来源：http://hz.jqgfzy.top/gthgfiwhna.html

if let n = opt { print(n) }
来源：http://hz.jqgufenzy.top/gtkfsekhdr.html

[T20] Swift：数组操作
来源：http://hz.9152youxi.cn/gtvirskovp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sufxvd.cn/gtqcjgiaua.html

[T21] Swift：遍历
来源：http://hz.gzhubu.top/gtyoyesflq.html

for x in a { print(x) }
来源：http://hz.shangyingyoupin.top/gtuqekfuij.html

[T22] Swift：字典
来源：http://hz.aibaodan.cn/gtamkzydoe.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnqzz.top/gtaxouyumi.html

[T23] Swift：函数
来源：http://hz.xinyue.icu/gtybugnhfi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cdnleiting.top/gthulnzvbw.html

[T24] Swift：闭包
来源：http://hz.xingfuxueyuan.xyz/gtfvaerjst.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj202588.top/gtfmhmyblg.html

[T25] Swift：结构体
来源：http://hz.snrcjt.cn/gtoatykvey.html

struct P { var x: Int }
来源：http://hz.hfpthk.cn/gticpjebxv.html

[T26] Swift：类与重写
来源：http://hz.zycfv.cn/gtrfdswnss.html

class A: Base { override func f() {} }
来源：http://hz.gaohongyu789.top/gtkvkkrhwi.html

[T27] Swift：错误处理
来源：http://hz.kuanghao11.cn/gtbfdohhnh.html

do { try f() } catch { print(error) }
来源：http://hz.cucudq.cn/gtlnextgyq.html

[T28] Swift：枚举
来源：http://hz.ydjk.org.cn/gtuxgccvrw.html

enum Color { case red, green }
来源：http://hz.yj20258.top/gtcokgnmrr.html

[T29] Swift：guard 提前返回
来源：http://hz.0kj1m.cn/gtxyqpmrzw.html

guard let x = opt else { return }
来源：http://hz.guannengcc.top/gtbwgqurwf.html

[T30] Swift：协议
来源：http://hz.jiagoushi.top/gtdfyeyito.html

protocol Shape { func area() -> Double }
来源：http://hz.aibaodan.cn/gtbhgygkmz.html

[T31] Lua：Hello World
来源：http://hz.smart0.xyz/gtvjsylqov.html

print("Hello")
来源：http://hz.nanxinkj.top/gtexrbzhmw.html

[T32] Lua：局部变量
来源：http://hz.xingfuxueyuan.xyz/gteviaikha.html

local a = 1
来源：http://hz.zhijiandao.cn/gtdrboqlbg.html

[T33] Lua：表（数组）
来源：http://hz.xuetiantiany.cn/gthdyvavas.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.tanke756.top/gttvswotks.html

[T34] Lua：遍历表
来源：http://hz.guowangkeji.top/gtgzygrgeo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.aizwys.cn/gtwyhtsoig.html

[T35] Lua：字典表
来源：http://hz.yongpay.top/gtaxiigdmr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhengqikj.top/gtbrnnweej.html

[T36] Lua：函数
来源：http://hz.yvedp.cn/gtmbgubgny.html

function add(a, b) return a + b end
来源：http://hz.ywan-chungtsiang.top/gtlkfswmst.html

[T37] Lua：字符串拼接
来源：http://hz.cqqwz.cn/gtavlcyagn.html

"a" .. "b"
来源：http://hz.ydzc1.top/gtlwzuztem.html

[T38] Lua：条件
来源：http://hz.guowangkeji.top/gtikkivcot.html

if x > 0 then print("正") end
来源：http://hz.nanxinkj.top/gtqwpcfklp.html

[T39] Lua：模式匹配
来源：http://hz.hywenlv.cn/gtxjuogfjs.html

string.find(s, "%d+")
来源：http://hz.xingfuxueyuan.xyz/gtkymlxqer.html

[T40] Lua：元表
来源：http://hz.yonumen.top/gtztqbpidu.html

setmetatable({}, { __index = base })
来源：http://hz.aizwys.cn/gtqtvvritf.html

[T41] Perl：Hello World
来源：http://hz.sysykeji.top/gtrglyqabe.html

print "Hello\n";
来源：http://hz.shzxlz.cn/gtulkjuztw.html

[T42] Perl：变量类型
来源：http://hz.yj202588.top/gtqbmlxzmk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fengsongda.top/gtkpyavhgx.html

[T43] Perl：字符串插值
来源：http://hz.ybcxt.top/gtkaryvraj.html

"值: $a"
来源：http://hz.ehwqpu.com/gtidyzlpub.html

[T44] Perl：条件
来源：http://hz.zycfv.cn/gtwmtgskcc.html

if ($a > 0) { print "正"; }
来源：http://hz.daxiang520.top/gtbcbbwewy.html

[T45] Perl：数组遍历
来源：http://hz.jlsjyb.cn/gteckzoobv.html

for my $x (@arr) { print $x; }
来源：http://hz.zhixingplan.top/gtpmdvpwpj.html

[T46] Perl：哈希操作
来源：http://hz.xziqi.cn/gtmyueursa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.nanxuanxn.top/gtbecrgugs.html

[T47] Perl：正则捕获
来源：http://hz.yj20258.top/gtskhjztbn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xylfe.cn/gtlnkyjeed.html

[T48] Perl：正则替换
来源：http://hz.vqdsnc.cn/gtrbzjlbvx.html

$s =~ s/old/new/g;
来源：http://hz.yj20258888.top/gttskuczny.html

[T49] Perl：函数
来源：http://hz.pycfn.com/gtgdgwgvex.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.meibo888.top/gtsgxayefq.html

[T50] Perl：逐行读文件
来源：http://hz.pycfn.com/gtxmcovfwc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yuanzhike.top/gtjifyohbb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhongyouzk.top/gtywyxmvew.html

[T51] Scala：Hello World
来源：http://hz.guowangkeji.top/gtqoyjmzyn.html

println("Hello")
来源：http://hz.jiagoushi.top/gtyqfkxhbi.html

[T52] Scala：变量
来源：http://hz.shanyushiyangtech.top/gtyflhhscc.html

val a = 1;  var b = 2
来源：http://hz.ehwqpu.com/gtvpnlnuuo.html

[T53] Scala：字符串插值
来源：http://hz.tianlin.xyz/gtelqrarnb.html

s"值: $b"
来源：http://hz.jqgufenzy.top/gtkhinfixu.html

[T54] Scala：集合映射
来源：http://hz.yangfankeji.com/gtwmjtmqky.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.vqdsnc.cn/gthihejpla.html

[T55] Scala：集合过滤
来源：http://hz.jlsjyb.cn/gtxmomrpku.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.pengpengdd.cyou/gtaqmvlayi.html

[T56] Scala：样例类
来源：http://hz.chenjidiqi.icu/gtuhtimsuf.html

case class User(name: String, age: Int)
来源：http://hz.vqdsnc.cn/gtjusajegb.html

[T57] Scala：模式匹配
来源：http://hz.fzhhl.top/gtiycfhwmr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ydzc1.top/gtqdfsrvka.html

[T58] Scala：函数定义
来源：http://hz.zhiwuduotai.top/gtmbixqkph.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ehwqpu.com/gtnhijfjpz.html

[T59] Scala：循环
来源：http://hz.chenzaomai.com/gtecjwnchv.html

for (i <- 1 to 10) println(i)
来源：http://hz.shzxlz.cn/gtxhoydssh.html

[T60] Scala：折叠
来源：http://hz.jqgufenzy.top/gtubugbxcc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yj20258888.top/gtckkvfvvx.html

================================================================================
来源：http://hz.tian-w.cn/gtfvghggaz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jqgufenzy.top/gtajunsnll.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gthabmytap.html

[U01] Py：创建虚拟环境
来源：http://hz.zhoulong.xyz/gtbmscxejr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.aibaodan.cn/gtsmakmnmj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ehwqpu.com/gtpxbasoah.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.quarkkingdee.top/gtubmxfdnv.html

[U03] Py：加载 .env 配置
来源：http://hz.cucudq.cn/gtaljclczz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shanyushiyangkeji.top/gtaabxmhow.html

[U04] Py：变量调试打印
来源：http://hz.guowangkeji.top/gtxqtndxpo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258888.top/gtyuiddcon.html

[U05] Py：列表去重且保序
来源：http://hz.c1oappe.top/gtltizkvgp.html

list(dict.fromkeys(arr))
来源：http://hz.xuetiantiany.cn/gtetdpqbrl.html

[U06] Py：合并两个字典
来源：http://hz.sysykeji.top/gtcgmbllwb.html

{**a, **b}
来源：http://hz.9152youxi.cn/gthsugbgpf.html

[U07] Py：反转字典键值
来源：http://hz.zhiwuduotai.top/gtmfrjbogv.html

{v: k for k, v in d.items()}
来源：http://hz.tanke756.top/gtuopgrpzy.html

[U08] Py：展平二维列表
来源：http://hz.316326.xyz/gttoaqpwix.html

[y for x in nested for y in x]
来源：http://hz.dianchejie.cn/gtbeprdxho.html

[U09] Py：字典取最大值的键
来源：http://hz.yonumen.top/gtzuvcosnn.html

max(d, key=d.get)
来源：http://hz.ybcxt.top/gtgrhoasaq.html

[U10] Py：按值排序字典
来源：http://hz.zhengqikj.top/gtfvdbjcsr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.aizwys.cn/gtyldfextz.html

[U11] Py：生成器表达式
来源：http://hz.jlsjyb.cn/gtiyacnwpj.html

(x * 2 for x in arr)
来源：http://hz.xingfuxueyuan.xyz/gtidtidibj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.havefunace.top/gtohnnyexa.html

Counter(arr).most_common(3)
来源：http://hz.ydzc1.top/gtobfwebra.html

[U13] Py：固定长度队列
来源：http://hz.aibaodan.cn/gtbaeaxbii.html

deque(maxlen=10)
来源：http://hz.havefunace.top/gtwsweimmr.html

[U14] Py：分组收集到列表
来源：http://hz.xinyue.icu/gtblyrxsxx.html

defaultdict(list)
来源：http://hz.ydzc1.top/gtpigjvsjv.html

[U15] Py：高精度计时
来源：http://hz.iojbl.cn/gtucgtkydr.html

t = time.perf_counter()
来源：http://hz.yuanzhike.top/gtpihshdbl.html

[U16] Py：命令行参数解析
来源：http://hz.zycfv.cn/gtxcqeqixa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.svipenyu.cn/gtcoscsxab.html

[U17] Py：初始化日志
来源：http://hz.yuanzhike.top/gtzlymivle.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yangfankeji.com/gtaynrrwgt.html

[U18] Py：预编译正则
来源：http://hz.gzhubu.top/gtsbkgwltb.html

pat = re.compile(r"\d+")
来源：http://hz.cdnleiting.top/gtpeysrywd.html

[U19] Py：正则替换带回调
来源：http://hz.fengsongda.top/gtifxksyhp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.pycfn.com/gtcwuglont.html

[U20] Py：缓存函数结果
来源：http://hz.sufxvd.cn/gtfithrrqg.html

@functools.lru_cache(maxsize=None)
来源：http://hz.vqdsnc.cn/gtgcybrrlj.html

[U21] Py：自定义上下文管理器
来源：http://hz.ppjwa.cn/gtnrfbiddu.html

@contextlib.contextmanager
来源：http://hz.yj20258.top/gtwggoyjux.html

[U22] Py：矩阵转置
来源：http://hz.jinqigfzy.top/gtxhqruijy.html

list(zip(*m))
来源：http://hz.mhx1999.top/gtpqodmlqr.html

[U23] Py：分块读取大文件
来源：http://hz.sxryk.cn/gtrrtyihaq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.vqdsnc.cn/gtjntnwati.html

[U24] Py：路径操作
来源：http://hz.jianghu66.top/gtwfernyuu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xziqi.cn/gtrebcnrxb.html

[U25] Py：CSV 按字典读
来源：http://hz.jinqigfzy.top/gtokerpqhe.html

csv.DictReader(f)
来源：http://hz.jinghuilouyu.cn/gtlyxkuzvb.html

[U26] Py：并发下载
来源：http://hz.daxiang520.top/gtngsjghgj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.andypj.xyz/gtnmtlpegk.html

[U27] Py：异步 HTTP
来源：http://hz.hywenlv.cn/gttafasuau.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.dianchejie.cn/gtxjoedkjf.html

[U28] Py：类型别名
来源：http://hz.ivvv.top/gtfkeldqic.html

UserId = int
来源：http://hz.aibaodan.cn/gtjspcqaym.html

[U29] Py：属性校验
来源：http://hz.gotoacloud.top/gtihnioktc.html

@property 与 @x.setter 配合
来源：http://hz.chenzaomai.com/gtmgisbewn.html

[U30] Py：数据类
来源：http://hz.cashguo.top/gthtmvtuvn.html

@dataclass(slots=True)
来源：http://hz.cdnleiting.top/gtqketescj.html

[U31] Py：单测
来源：http://hz.yanxiufei.cn/gtxixzqqrr.html

python -m pytest -q
来源：http://hz.nanxuanxn.top/gtojdhvxwa.html

[U32] Py：代码格式化
来源：http://hz.xuetiantiany.cn/gtnicaxaab.html

ruff format . && ruff check --fix .
来源：http://hz.yueranfly.top/gtueldtvqx.html

[U33] Py：打包发布
来源：http://hz.tianlin.xyz/gtxowqbcnq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jyoumei.cn/gtoeoowyzh.html

[U34] Py：判断编码
来源：http://hz.bjfxy.top/gtcklryvus.html

chardet.detect(raw)
来源：http://hz.ydzc1.top/gtiznwbnsl.html

[U35] Py：发送邮件
来源：http://hz.svipenyu.cn/gtsgwvvyvp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.tianlin.xyz/gtaonncojv.html

[U36] Py：定时任务
来源：http://hz.zdqjudy.top/gtxtfvohew.html

schedule.every(10).minutes.do(job)
来源：http://hz.sxryk.cn/gtiqdhgokn.html

[U37] Py：读写 Excel
来源：http://hz.ppjwa.cn/gtkeslortu.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.c1oappe.top/gtdhykwveu.html

[U38] Py：获取脚本所在目录
来源：http://hz.0kj1m.cn/gtvnowuufy.html

Path(__file__).resolve().parent
来源：http://hz.daria6918.cn/gtndzdpodf.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhijiandao.cn/gtxeshtktg.html

sys.stdout.isatty()
来源：http://hz.xziqi.cn/gtfaemiefk.html

[U40] Py：打印到标准错误
来源：http://hz.svipenyu.cn/gtabfkfwhw.html

print("err", file=sys.stderr)
来源：http://hz.kuanghao11.cn/gtqnqkueid.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ydjk.org.cn/gterdgutvi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinqigufen.top/gtrxchxfrf.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jqgufenzy.top/gtentbypgd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.cdnleiting.top/gtkcfoiifl.html

[U43] PHP：声明命名空间
来源：http://hz.daxiang520.top/gtizcoaqki.html

namespace App\Http;
来源：http://hz.yueranfly.top/gtzubplgnc.html

[U44] PHP：开启严格类型
来源：http://hz.xziqi.cn/gtdvoobzev.html

declare(strict_types=1);
来源：http://hz.zdqjudy.top/gtgpzthkfv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xziqi.cn/gtlvuhajca.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.birdmap.top/gtwcdbnjmb.html

[U46] PHP：可空类型
来源：http://hz.jianghu66.top/gtwzywrnia.html

?string $name = null
来源：http://hz.ybcxt.top/gtwbczrrdn.html

[U47] PHP：联合类型
来源：http://hz.nanxuanxn.top/gtudkxgesa.html

int|string $id
来源：http://hz.xinyue.icu/gtahjpfmzy.html

[U48] PHP：纯枚举
来源：http://hz.hnqzz.top/gtqedftmjh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gotoacloud.top/gtyjcwjywb.html

[U49] PHP：只读属性
来源：http://hz.dashuyun.cn/gtmkliqupa.html

public readonly string $name
来源：http://hz.jinghuilouyu.cn/gtzeimfpap.html

[U50] PHP：构造器属性提升
来源：http://hz.vqdsnc.cn/gtgqnrwdno.html

public function __construct(private int $id) {}
来源：http://hz.feifeiyinyue.top/gtnlouipvr.html

[U51] PHP：数组解构
来源：http://hz.pengpengdd.cyou/gtsjuwzjnt.html

[$a, $b] = $arr;
来源：http://hz.shzxlz.cn/gtgbphmrer.html

[U52] PHP：箭头函数
来源：http://hz.dianchejie.cn/gtgkhcrfuf.html

$double = fn($x) => $x * 2;
来源：http://hz.snrcjt.cn/gtfikeuhgu.html

[U53] PHP：空合并运算符
来源：http://hz.aizwys.cn/gtzybbdnms.html

$v = $a ?? $b ?? "default";
来源：http://hz.shangyingyoupin.top/gtpfcckhid.html

[U54] PHP：空安全调用
来源：http://hz.yanxiufei.cn/gtjqqlmmrn.html

$obj?->method()
来源：http://hz.tian-w.cn/gtgcmupeim.html

[U55] PHP：match 表达式
来源：http://hz.gaohongyu789.top/gtoxpzquie.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.316326.xyz/gtzfjoddoh.html

[U56] PHP：命名参数
来源：http://hz.xuanzx.com/gtbsylsjpx.html

f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtltzrnyva.html

[U57] PHP：字符串插值
来源：http://hz.gzhubu.top/gttkvkrfho.html

"值: {$a}"
来源：http://hz.jlsjyb.cn/gthwrfwuqj.html

[U58] PHP：数组三件套
来源：http://hz.guowangkeji.top/gtmnjudeuq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hnqzz.top/gttgugbvcg.html

[U59] PHP：自定义排序
来源：http://hz.pengpengdd.cyou/gtudfyccka.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fzhhl.top/gtgrtkvxsl.html

[U60] PHP：JSON 编解码
来源：http://hz.zhoulong.xyz/gtrmbhnihf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cheryme.top/gtopcvdwwc.html

[U61] PHP：正则
来源：http://hz.xylfe.cn/gtjbjencgw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtnanikilu.html

[U62] PHP：日期对象
来源：http://hz.ppjwa.cn/gtxvxmdhcn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.quarkkingdee.top/gtqxwxdawl.html

[U63] PHP：文件读写
来源：http://hz.guannengcc.top/gtxutyjsqi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yonumen.top/gtmkjdcqgt.html

[U64] PHP：目录遍历
来源：http://hz.jqgfzy.top/gtbngelspl.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jlsjyb.cn/gtyjznlbfx.html

[U65] PHP：会话
来源：http://hz.tian-w.cn/gtsihgeloz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.tianlin.xyz/gtvvymbbpv.html

[U66] PHP：设置 Cookie
来源：http://hz.nanxuanxn.top/gtefekdttm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gogol.net.cn/gtnotgwrxd.html

[U67] PHP：处理文件上传
来源：http://hz.meibo888.top/gtcljnwcsu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yangfankeji.com/gtpzwnypwc.html

[U68] PHP：PDO 连接
来源：http://hz.zhengqikj.top/gtgnvknaqd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhengqikj.top/gtxsgmnorj.html

[U69] PHP：PDO 预处理
来源：http://hz.shanyushiyangtech.top/gthmrqgoit.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.chenlongwang.top/gtkdeoyxcj.html

[U70] PHP：PDO 事务
来源：http://hz.zhoulong.xyz/gtyizcjtpj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yvedp.cn/gtycghphxr.html

[U71] PHP：抛出异常
来源：http://hz.sufxvd.cn/gtdbnbmftj.html

throw new RuntimeException("失败", 500);
来源：http://hz.ywan-chungtsiang.top/gtxhtsrhbc.html

[U72] PHP：写错误日志
来源：http://hz.ehwqpu.com/gtwnulkwdn.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jyoumei.cn/gtinrzuftv.html

[U73] PHP：读取 ini 配置
来源：http://hz.hnqzz.top/gtaczwishl.html

parse_ini_file("config.ini", true)
来源：http://hz.gotoacloud.top/gtubttczgz.html

[U74] PHP：读取环境变量
来源：http://hz.jqgufenzy.top/gtjifqypkx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.0kj1m.cn/gtqbdefxso.html

[U75] PHP：依赖注入
来源：http://hz.hongshengwenyu.top/gtajpjlkcq.html

composer require psr/container
来源：http://hz.zhixingplan.top/gtfiubhxot.html

[U76] PHP：简单路由
来源：http://hz.shangyingyoupin.top/gtygwqajpz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yangfankeji.com/gtaiaylsch.html

[U77] PHP：模板渲染
来源：http://hz.zdqjudy.top/gtkotinabl.html

composer require twig/twig
来源：http://hz.xinyue.icu/gtpgkkhsim.html

[U78] PHP：单元测试
来源：http://hz.daxiang520.top/gtrwpktauy.html

composer require --dev phpunit/phpunit
来源：http://hz.gogol.net.cn/gtkuhenjui.html

[U79] PHP：静态分析
来源：http://hz.tianlin.xyz/gtddzcqrek.html

composer require --dev phpstan/phpstan
来源：http://hz.yueranfly.top/gtwljeroqx.html

[U80] PHP：代码规范修复
来源：http://hz.cqqwz.cn/gtuxnpocow.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhoulong.xyz/gtconecvos.html

[U81] JS：初始化项目
来源：http://hz.birdmap.top/gttolcnaoi.html

npm init -y;  npm i express
来源：http://hz.meibo888.top/gteyzfwqfy.html

[U82] JS：package.json 脚本
来源：http://hz.yj20258888.top/gttjwkobix.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yvedp.cn/gtoizdrehb.html


<!-- 参考信息 -->