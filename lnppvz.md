代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://hz.quarkkingdee.top/gthelnsmzy.html

[S59] C++：静态断言
来源：http://hz.ehwqpu.com/gtqkfyxtzk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj20258888.top/gtzcqeskkb.html

[S60] C++：遍历并删除元素
来源：http://hz.xuetiantiany.cn/gtektajnrk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shzxlz.cn/gtzvbnalea.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gthoiymjng.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenlongwang.top/gtdaemonun.html

================================================================================
来源：http://hz.ivvv.top/gtagpqlhjm.html

[T01] Kotlin：Hello World
来源：http://hz.hnxiangtu.top/gtbgqzabgr.html

println("Hello")
来源：http://hz.hywenlv.cn/gtomtbzcav.html

[T02] Kotlin：变量
来源：http://hz.sxryk.cn/gterxuanzc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shuidangran.top/gtzcxsrjon.html

[T03] Kotlin：字符串模板
来源：http://hz.ehwqpu.com/gtcjoutvrh.html

"值: $b"
来源：http://hz.316326.xyz/gtexghcslf.html

[T04] Kotlin：空安全
来源：http://hz.hammf.cn/gtvnedenog.html

val n: String? = null;  n?.length
来源：http://hz.tianlin.xyz/gtpwszxrda.html

[T05] Kotlin：when 表达式
来源：http://hz.zhongyouzk.top/gteeehoqqj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.52xcode.cn/gtyodnpkch.html

[T06] Kotlin：集合映射
来源：http://hz.zdqjudy.top/gtbuixdokb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hongshengwenyu.top/gtjjohkqjv.html

[T07] Kotlin：集合过滤
来源：http://hz.cucudq.cn/gtdyyriwmv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.meibo888.top/gtzapegcsm.html

[T08] Kotlin：数据类
来源：http://hz.sysykeji.top/gtgxyvynsb.html

data class User(val name: String, val age: Int)
来源：http://hz.ehwqpu.com/gtbhseakar.html

[T09] Kotlin：扩展函数
来源：http://hz.ehwqpu.com/gtvhahlwqp.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtmghrfryr.html

[T10] Kotlin：默认参数
来源：http://hz.sufxvd.cn/gthudoalca.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.bjfxy.top/gtxqrqkdfy.html

[T11] Kotlin：协程
来源：http://hz.jiagoushi.top/gthjvyfuzb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hysaishi.cn/gtyxbqpihe.html

[T12] Kotlin：解构声明
来源：http://hz.yuanzhike.top/gttxfgaaax.html

val (a, b) = Pair(1, 2)
来源：http://hz.dianchejie.cn/gtzbotygts.html

[T13] Kotlin：只读 Map
来源：http://hz.xylfe.cn/gtuobofhtt.html

val m = mapOf("a" to 1)
来源：http://hz.nwbrower.top/gtvxfjnbtv.html

[T14] Kotlin：循环
来源：http://hz.jqgufenzy.top/gtbeihjusk.html

for (i in 1..10) println(i)
来源：http://hz.xziqi.cn/gtriypfooh.html

[T15] Kotlin：接口
来源：http://hz.cashguo.top/gtbpcefqqo.html

interface Shape { fun area(): Double }
来源：http://hz.c1oappe.top/gtgkzeqkhh.html

[T16] Swift：Hello World
来源：http://hz.yanxiufei.cn/gtprzmaone.html

print("Hello")
来源：http://hz.sufxvd.cn/gthodgbwmj.html

[T17] Swift：变量与常量
来源：http://hz.fzhhl.top/gtnuyzoziw.html

var a = 1;  let b = 2
来源：http://hz.feifeiyinyue.top/gtnhnywrnk.html

[T18] Swift：字符串插值
来源：http://hz.dianchejie.cn/gthyqveuru.html

"值: \(b)"
来源：http://hz.hywenlv.cn/gtmzfbokev.html

[T19] Swift：可选绑定
来源：http://hz.0kj1m.cn/gtyrpqsskw.html

if let n = opt { print(n) }
来源：http://hz.gzhubu.top/gtzxsoluyb.html

[T20] Swift：数组操作
来源：http://hz.ydjk.org.cn/gtumyyidgb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.haohaochexian.top/gtynvvizrj.html

[T21] Swift：遍历
来源：http://hz.nwbrower.top/gtdmqwophq.html

for x in a { print(x) }
来源：http://hz.shanyushiyangkeji.top/gtmsqoukcq.html

[T22] Swift：字典
来源：http://hz.wangshuangyany.cn/gtdzegfljl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.kuanghao11.cn/gtfkziejhw.html

[T23] Swift：函数
来源：http://hz.tianlin.xyz/gtlupeehwd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.daxiang520.top/gtzncbtsst.html

[T24] Swift：闭包
来源：http://hz.yanxiufei.cn/gtjaoxgsqk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cucudq.cn/gtyvhtuyey.html

[T25] Swift：结构体
来源：http://hz.sufxvd.cn/gtdbgbhodc.html

struct P { var x: Int }
来源：http://hz.jinghuilouyu.cn/gtfolhkmbs.html

[T26] Swift：类与重写
来源：http://hz.tian-w.cn/gtxycjxmug.html

class A: Base { override func f() {} }
来源：http://hz.yonumen.top/gtopjnmwfq.html

[T27] Swift：错误处理
来源：http://hz.jiagoushi.top/gtflylybyp.html

do { try f() } catch { print(error) }
来源：http://hz.yvedp.cn/gthafvwmmn.html

[T28] Swift：枚举
来源：http://hz.hongshengwenyu.top/gtfqsysmps.html

enum Color { case red, green }
来源：http://hz.chenzaomai.com/gtndryblnu.html

[T29] Swift：guard 提前返回
来源：http://hz.yj20258888.top/gtmxvsxacf.html

guard let x = opt else { return }
来源：http://hz.zycfv.cn/gtrrbzefre.html

[T30] Swift：协议
来源：http://hz.ydjk.org.cn/gtinngswzc.html

protocol Shape { func area() -> Double }
来源：http://hz.zhoulong.xyz/gtvdntauaw.html

[T31] Lua：Hello World
来源：http://hz.smart0.xyz/gtxsgfihco.html

print("Hello")
来源：http://hz.dianchejie.cn/gtnzcbgqsh.html

[T32] Lua：局部变量
来源：http://hz.xinyue.icu/gtbbwojifg.html

local a = 1
来源：http://hz.c1oappe.top/gtungsitdc.html

[T33] Lua：表（数组）
来源：http://hz.zdqjudy.top/gtbreswqda.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.fengsongda.top/gtgpxvebde.html

[T34] Lua：遍历表
来源：http://hz.feifeiyinyue.top/gtqgmqegcl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yj202588.top/gtyiucbuxz.html

[T35] Lua：字典表
来源：http://hz.aibaodan.cn/gtueqpnuhm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhijiandao.cn/gtvyykosvt.html

[T36] Lua：函数
来源：http://hz.c1oappe.top/gtedkzsdzv.html

function add(a, b) return a + b end
来源：http://hz.hnxiangtu.top/gtxusenrdh.html

[T37] Lua：字符串拼接
来源：http://hz.bjfxy.top/gtiwtyvkge.html

"a" .. "b"
来源：http://hz.fzhhl.top/gtpssisogw.html

[T38] Lua：条件
来源：http://hz.cucudq.cn/gtpedpfifw.html

if x > 0 then print("正") end
来源：http://hz.xziqi.cn/gtxaigmypt.html

[T39] Lua：模式匹配
来源：http://hz.cucudq.cn/gtompyxzex.html

string.find(s, "%d+")
来源：http://hz.yj202588.top/gtrfixgvog.html

[T40] Lua：元表
来源：http://hz.chenjidiqi.icu/gtcjpeurfx.html

setmetatable({}, { __index = base })
来源：http://hz.316326.xyz/gtrxtpuiwj.html

[T41] Perl：Hello World
来源：http://hz.nwbrower.top/gtoixyzttc.html

print "Hello\n";
来源：http://hz.zhengqikj.top/gtigtsebcc.html

[T42] Perl：变量类型
来源：http://hz.xingfuxueyuan.xyz/gtktgkexbd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhijiandao.cn/gtqzpefvpn.html

[T43] Perl：字符串插值
来源：http://hz.cucudq.cn/gtjpjfnvry.html

"值: $a"
来源：http://hz.316326.xyz/gtijybhxpr.html

[T44] Perl：条件
来源：http://hz.hnqzz.top/gttppxtiqm.html

if ($a > 0) { print "正"; }
来源：http://hz.dianchejie.cn/gtrwfpdypb.html

[T45] Perl：数组遍历
来源：http://hz.ydjk.org.cn/gtuimccutu.html

for my $x (@arr) { print $x; }
来源：http://hz.zdqjudy.top/gtzlinqiqd.html

[T46] Perl：哈希操作
来源：http://hz.yj20258888.top/gtgcwjenmr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hnxiangtu.top/gthwllmfvd.html

[T47] Perl：正则捕获
来源：http://hz.hysaishi.cn/gttdcawjbs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.9152youxi.cn/gtdurcowez.html

[T48] Perl：正则替换
来源：http://hz.gaohongyu789.top/gtqfgpgrtn.html

$s =~ s/old/new/g;
来源：http://hz.tianlin.xyz/gtpipbunvi.html

[T49] Perl：函数
来源：http://hz.andypj.xyz/gtpmzjvxhf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hywenlv.cn/gtelitkizv.html

[T50] Perl：逐行读文件
来源：http://hz.sysykeji.top/gtdcblfxru.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ehwqpu.com/gtsaldseig.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xziqi.cn/gtmhkrvrzn.html

[T51] Scala：Hello World
来源：http://hz.0kj1m.cn/gtqyvdnosb.html

println("Hello")
来源：http://hz.xuetiantiany.cn/gtwzbipbah.html

[T52] Scala：变量
来源：http://hz.yj202588.top/gtlminokcg.html

val a = 1;  var b = 2
来源：http://hz.cashguo.top/gtrcrzcbni.html

[T53] Scala：字符串插值
来源：http://hz.tanke756.top/gtnrgwmjza.html

s"值: $b"
来源：http://hz.smart0.xyz/gtjijlomyb.html

[T54] Scala：集合映射
来源：http://hz.andypj.xyz/gtxxxyrorg.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jianghu66.top/gtfhemhwwn.html

[T55] Scala：集合过滤
来源：http://hz.dashuyun.cn/gtnpsflzwo.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.chenlongwang.top/gtrqrwliry.html

[T56] Scala：样例类
来源：http://hz.tian-w.cn/gtjnpizsnh.html

case class User(name: String, age: Int)
来源：http://hz.jyoumei.cn/gthljyyusw.html

[T57] Scala：模式匹配
来源：http://hz.cheryme.top/gtgsjozoxt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cqqwz.cn/gtjdfgtsck.html

[T58] Scala：函数定义
来源：http://hz.meibo888.top/gtuydbqhvd.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cdnleiting.top/gtobtfegwp.html

[T59] Scala：循环
来源：http://hz.iojbl.cn/gtikdhgdeo.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhixingplan.top/gtcwkxexdq.html

[T60] Scala：折叠
来源：http://hz.wangdashe.top/gttqelpjji.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jiagoushi.top/gtmqdoqwmr.html

================================================================================
来源：http://hz.wangdashe.top/gtrnnwnauo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yueranfly.top/gttfhvgfyp.html

================================================================================
来源：http://hz.vqdsnc.cn/gtiaztjnpp.html

[U01] Py：创建虚拟环境
来源：http://hz.hnqzz.top/gtjyggayfo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xuetiantiany.cn/gtzehlbbmo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.guannengcc.top/gtpmvibjmq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yuanzhike.top/gtqzwnxdxn.html

[U03] Py：加载 .env 配置
来源：http://hz.jinghuilouyu.cn/gtlaaqzslq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhongyouzk.top/gthxmjkddi.html

[U04] Py：变量调试打印
来源：http://hz.hnqzz.top/gtbybtkjgg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nanxuanxn.top/gtrmwucena.html

[U05] Py：列表去重且保序
来源：http://hz.hfpthk.cn/gtdqklfmua.html

list(dict.fromkeys(arr))
来源：http://hz.hnqzz.top/gtdwolqrrd.html

[U06] Py：合并两个字典
来源：http://hz.52xcode.cn/gtkvpjtsgh.html

{**a, **b}
来源：http://hz.zdqjudy.top/gtqegmytgb.html

[U07] Py：反转字典键值
来源：http://hz.jiagoushi.top/gtixzczdux.html

{v: k for k, v in d.items()}
来源：http://hz.dashuyun.cn/gtwxxeolhl.html

[U08] Py：展平二维列表
来源：http://hz.yongpay.top/gtdkdrmvkz.html

[y for x in nested for y in x]
来源：http://hz.dashuyun.cn/gtczjifimu.html

[U09] Py：字典取最大值的键
来源：http://hz.zdqjudy.top/gthcsxqkvp.html

max(d, key=d.get)
来源：http://hz.ybcxt.top/gtebgcnwgj.html

[U10] Py：按值排序字典
来源：http://hz.hammf.cn/gtiuilqjki.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nanxuanxn.top/gtruusalsr.html

[U11] Py：生成器表达式
来源：http://hz.shuidangran.top/gtjmuxdyat.html

(x * 2 for x in arr)
来源：http://hz.jyoumei.cn/gtfouklnyr.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tanke756.top/gteqelmrfs.html

Counter(arr).most_common(3)
来源：http://hz.sufxvd.cn/gtboexzbxl.html

[U13] Py：固定长度队列
来源：http://hz.jqgufenzy.top/gtvhrayipb.html

deque(maxlen=10)
来源：http://hz.jinyuanbaomall.cn/gtykrzsuli.html

[U14] Py：分组收集到列表
来源：http://hz.jqgfzy.top/gtkmhlrpkj.html

defaultdict(list)
来源：http://hz.jiagoushi.top/gtksnplafy.html

[U15] Py：高精度计时
来源：http://hz.yuxming.cn/gtrjxbpwmw.html

t = time.perf_counter()
来源：http://hz.quarkkingdee.top/gtpcwmcglc.html

[U16] Py：命令行参数解析
来源：http://hz.zycfv.cn/gtjviyksxe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.dianchejie.cn/gtujjzxjnv.html

[U17] Py：初始化日志
来源：http://hz.316326.xyz/gtdmzfgvpp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.gaohongyu789.top/gtwdlakdvt.html

[U18] Py：预编译正则
来源：http://hz.yangfankeji.com/gtrqsodxid.html

pat = re.compile(r"\d+")
来源：http://hz.snrcjt.cn/gtlairwgle.html

[U19] Py：正则替换带回调
来源：http://hz.sweek.top/gtskvvyugn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jiagoushi.top/gtgrgakhzv.html

[U20] Py：缓存函数结果
来源：http://hz.shanyushiyangkeji.top/gtuwjazeqg.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shanyushiyangtech.top/gthkqxjmhe.html

[U21] Py：自定义上下文管理器
来源：http://hz.chenjidiqi.icu/gtoqyseymo.html

@contextlib.contextmanager
来源：http://hz.ivvv.top/gtvibfbwoo.html

[U22] Py：矩阵转置
来源：http://hz.cdnleiting.top/gtyqervwul.html

list(zip(*m))
来源：http://hz.sysykeji.top/gtdpfdnhuv.html

[U23] Py：分块读取大文件
来源：http://hz.havefunace.top/gtzqkhpaqx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cqqwz.cn/gtgfquntwy.html

[U24] Py：路径操作
来源：http://hz.xingfuxueyuan.xyz/gtjtventmi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gzhubu.top/gtvyaupqhv.html

[U25] Py：CSV 按字典读
来源：http://hz.yuanzhike.top/gtvnqupuug.html

csv.DictReader(f)
来源：http://hz.fengsongda.top/gtcmejrich.html

[U26] Py：并发下载
来源：http://hz.nanxuanxn.top/gtxhfjmcaf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jlsjyb.cn/gtumxqtdzm.html

[U27] Py：异步 HTTP
来源：http://hz.xingfuxueyuan.xyz/gtqgaiosdt.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ydzc1.top/gtomyukfop.html

[U28] Py：类型别名
来源：http://hz.wangshuangyany.cn/gtqwntlxeg.html

UserId = int
来源：http://hz.zhijiandao.cn/gtnqkvohsl.html

[U29] Py：属性校验
来源：http://hz.tian-w.cn/gtjgfwuafu.html

@property 与 @x.setter 配合
来源：http://hz.jinghuilouyu.cn/gtbeglwvqn.html

[U30] Py：数据类
来源：http://hz.tian-w.cn/gtsqssqlmn.html

@dataclass(slots=True)
来源：http://hz.xinyue.icu/gtbcxpxudd.html

[U31] Py：单测
来源：http://hz.cheryme.top/gtmtwymocv.html

python -m pytest -q
来源：http://hz.52xcode.cn/gtbcjxlypf.html

[U32] Py：代码格式化
来源：http://hz.hnqzz.top/gttwtgaqez.html

ruff format . && ruff check --fix .
来源：http://hz.xinyue.icu/gtoynqjahu.html

[U33] Py：打包发布
来源：http://hz.tian-w.cn/gtqhtkhtkl.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhongyouzk.top/gtdfexvuob.html

[U34] Py：判断编码
来源：http://hz.jyoumei.cn/gtwdtdvlek.html

chardet.detect(raw)
来源：http://hz.chenzaomai.com/gtomcjuief.html

[U35] Py：发送邮件
来源：http://hz.yonumen.top/gtgjftfoxz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shzxlz.cn/gtepfkhwom.html

[U36] Py：定时任务
来源：http://hz.redwolf501.top/gtpnuwsikp.html

schedule.every(10).minutes.do(job)
来源：http://hz.jianghu66.top/gtgduxbfba.html

[U37] Py：读写 Excel
来源：http://hz.chenjidiqi.icu/gtiunxtebj.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xziqi.cn/gtjlvephmh.html

[U38] Py：获取脚本所在目录
来源：http://hz.jinqigufen.top/gtqhrbbqlx.html

Path(__file__).resolve().parent
来源：http://hz.shzxlz.cn/gtmvuqrocp.html

[U39] Py：判断是否在交互环境
来源：http://hz.snrcjt.cn/gtuqlrftiz.html

sys.stdout.isatty()
来源：http://hz.zdqjudy.top/gtvwqriyjs.html

[U40] Py：打印到标准错误
来源：http://hz.shangyingyoupin.top/gtydoxyzel.html

print("err", file=sys.stderr)
来源：http://hz.mhx1999.top/gtjdmoexoo.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yuanzhike.top/gtguqcaafr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.chenzaomai.com/gtnnnbwarp.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yanxiufei.cn/gtugbypgsf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jqgfzy.top/gtgqqjbyis.html

[U43] PHP：声明命名空间
来源：http://hz.cucudq.cn/gtxhkswfhk.html

namespace App\Http;
来源：http://hz.hysaishi.cn/gtsxulbhbq.html

[U44] PHP：开启严格类型
来源：http://hz.316326.xyz/gtrrkrsmid.html

declare(strict_types=1);
来源：http://hz.wangdashe.top/gtdisjbuqg.html

[U45] PHP：类型声明与返回类型
来源：http://hz.daria6918.cn/gtavzyrwya.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydzc1.top/gtrsdnqlcj.html

[U46] PHP：可空类型
来源：http://hz.hnqzz.top/gtpnpwzbmb.html

?string $name = null
来源：http://hz.cheryme.top/gtvqgpdqsh.html

[U47] PHP：联合类型
来源：http://hz.yuxming.cn/gtryqjylkp.html

int|string $id
来源：http://hz.sufxvd.cn/gtqnyarjtd.html

[U48] PHP：纯枚举
来源：http://hz.yvedp.cn/gtuepjkpyh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cheryme.top/gtpstcqclx.html

[U49] PHP：只读属性
来源：http://hz.ybcxt.top/gtdtbxadop.html

public readonly string $name
来源：http://hz.zycfv.cn/gtcvrxfles.html

[U50] PHP：构造器属性提升
来源：http://hz.yvedp.cn/gtggmzpwvb.html

public function __construct(private int $id) {}
来源：http://hz.redwolf501.top/gtrsftpdbr.html

[U51] PHP：数组解构
来源：http://hz.chenjidiqi.icu/gtvhkqqklv.html

[$a, $b] = $arr;
来源：http://hz.jinyuanbaomall.cn/gtezglxojd.html

[U52] PHP：箭头函数
来源：http://hz.pengpengdd.cyou/gtjpjcezuw.html

$double = fn($x) => $x * 2;
来源：http://hz.jqgfzy.top/gttanytkdb.html

[U53] PHP：空合并运算符
来源：http://hz.guannengcc.top/gtlydlptyk.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhoulong.xyz/gtaellfqpn.html

[U54] PHP：空安全调用
来源：http://hz.meibo888.top/gtlxnozadu.html

$obj?->method()
来源：http://hz.feifeiyinyue.top/gtftyjepvc.html

[U55] PHP：match 表达式
来源：http://hz.feifeiyinyue.top/gtnvxovpbk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xingfuxueyuan.xyz/gtmvwxnmtf.html

[U56] PHP：命名参数
来源：http://hz.shanyushiyangkeji.top/gtnprrddsc.html

f(a: 1, b: 2)
来源：http://hz.tian-w.cn/gtukdehrsy.html

[U57] PHP：字符串插值
来源：http://hz.zhoulong.xyz/gtstxmzoiv.html

"值: {$a}"
来源：http://hz.daxiang520.top/gtastsuldf.html

[U58] PHP：数组三件套
来源：http://hz.pycfn.com/gtgzxnsfkp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.mhx1999.top/gtgfnmdvsz.html

[U59] PHP：自定义排序
来源：http://hz.gogol.net.cn/gtwxnxmumm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nwbrower.top/gteplhsugi.html

[U60] PHP：JSON 编解码
来源：http://hz.havefunace.top/gtojatvbnd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xylfe.cn/gtrbvrdphn.html

[U61] PHP：正则
来源：http://hz.sweek.top/gtqjtlmqwx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gthobkemuj.html

[U62] PHP：日期对象
来源：http://hz.xuetiantiany.cn/gtmjtpibdf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.c1oappe.top/gtntwhfnte.html

[U63] PHP：文件读写
来源：http://hz.daxiang520.top/gtjmqbnard.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hnxiangtu.top/gtvxfnjeot.html

[U64] PHP：目录遍历
来源：http://hz.feifeiyinyue.top/gthfpjimjx.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.shuidangran.top/gtzpytyclb.html

[U65] PHP：会话
来源：http://hz.redwolf501.top/gtmhuyrjpn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.tianlin.xyz/gtrarqbsku.html

[U66] PHP：设置 Cookie
来源：http://hz.meibo888.top/gtgusqwmct.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.birdmap.top/gttbiuvqgl.html

[U67] PHP：处理文件上传
来源：http://hz.guannengcc.top/gtfuhigeyl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yongpay.top/gtxmvnqjro.html

[U68] PHP：PDO 连接
来源：http://hz.kuanghao11.cn/gtvqgiscgg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.sweek.top/gtxurrbzta.html

[U69] PHP：PDO 预处理
来源：http://hz.zhengqikj.top/gtgtdkbbkl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jyoumei.cn/gtplzbgflr.html

[U70] PHP：PDO 事务
来源：http://hz.sxryk.cn/gtgetubagz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hywenlv.cn/gtzqwxpkma.html

[U71] PHP：抛出异常
来源：http://hz.hnxiangtu.top/gtfdaxkvfv.html

throw new RuntimeException("失败", 500);
来源：http://hz.iojbl.cn/gtybiogaxx.html

[U72] PHP：写错误日志
来源：http://hz.jinyuanbaomall.cn/gthdbkrkdr.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cqqwz.cn/gtxmexgsxh.html

[U73] PHP：读取 ini 配置
来源：http://hz.xinyue.icu/gtyqwoqoby.html

parse_ini_file("config.ini", true)
来源：http://hz.nanxuanxn.top/gtlnqxhmqr.html

[U74] PHP：读取环境变量
来源：http://hz.gaohongyu789.top/gtjidytueu.html

getenv("APP_ENV") ?: "production"
来源：http://hz.daxiang520.top/gtfworetxn.html

[U75] PHP：依赖注入
来源：http://hz.smart0.xyz/gtmpnaoyew.html

composer require psr/container
来源：http://hz.bjfxy.top/gtthguqefn.html

[U76] PHP：简单路由
来源：http://hz.sweek.top/gtyeqpnfmn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zdqjudy.top/gtptlumjxt.html

[U77] PHP：模板渲染
来源：http://hz.gaohongyu789.top/gtrtxboyog.html

composer require twig/twig
来源：http://hz.zhaomingkeji.xyz/gtptrzsaoy.html

[U78] PHP：单元测试
来源：http://hz.xingfuxueyuan.xyz/gtkitnohoa.html

composer require --dev phpunit/phpunit
来源：http://hz.aibaodan.cn/gtkwceozno.html

[U79] PHP：静态分析
来源：http://hz.cucudq.cn/gtiwulsmjg.html

composer require --dev phpstan/phpstan
来源：http://hz.sxryk.cn/gtjkfqmdzl.html

[U80] PHP：代码规范修复
来源：http://hz.zdqjudy.top/gtrzyexbrm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sysykeji.top/gtzmbhfmeh.html

[U81] JS：初始化项目
来源：http://hz.snrcjt.cn/gtijrcjxli.html

npm init -y;  npm i express
来源：http://hz.zycfv.cn/gtwjeakcia.html

[U82] JS：package.json 脚本
来源：http://hz.mhx1999.top/gtfbawgkts.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hnqzz.top/gtauflrczu.html

[U83] JS：ES Module 导入导出
来源：http://hz.jinqigfzy.top/gtsdfhdzfd.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cashguo.top/gtsbyzauae.html

[U84] JS：CommonJS 写法
来源：http://hz.yangfankeji.com/gtbcaarhou.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hongshengwenyu.top/gtexfebzmu.html


<!-- 参考信息 -->