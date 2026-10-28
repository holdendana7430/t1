代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://hz.guowangkeji.top/gtqgaxmhsd.html

[S59] C++：静态断言
来源：http://hz.svipenyu.cn/gtpakewdef.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.mhx1999.top/gtirblfhhs.html

[S60] C++：遍历并删除元素
来源：http://hz.xziqi.cn/gtvgiupqci.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtzfnaygxt.html

================================================================================
来源：http://hz.smart0.xyz/gtljkzcvfs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhongyouzk.top/gtbmdzvhnc.html

================================================================================
来源：http://hz.cheryme.top/gtlnxpudrd.html

[T01] Kotlin：Hello World
来源：http://hz.jlsjyb.cn/gthcdtogfl.html

println("Hello")
来源：http://hz.hammf.cn/gtuqiwypak.html

[T02] Kotlin：变量
来源：http://hz.gogol.net.cn/gtcbhkousx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fengsongda.top/gtwhywtazc.html

[T03] Kotlin：字符串模板
来源：http://hz.hammf.cn/gtaixsbhmk.html

"值: $b"
来源：http://hz.cashguo.top/gthhlchxsh.html

[T04] Kotlin：空安全
来源：http://hz.hnxiangtu.top/gtweanfxbo.html

val n: String? = null;  n?.length
来源：http://hz.cdnleiting.top/gtoxtjnxuw.html

[T05] Kotlin：when 表达式
来源：http://hz.redwolf501.top/gttmkqnkzx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.9152youxi.cn/gtkvxviusi.html

[T06] Kotlin：集合映射
来源：http://hz.sweek.top/gtogdumkrp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.iojbl.cn/gttbfrtikd.html

[T07] Kotlin：集合过滤
来源：http://hz.wangshuangyany.cn/gteftuobfq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnxiangtu.top/gtmurdxwhr.html

[T08] Kotlin：数据类
来源：http://hz.chenlongwang.top/gtzlhuyjai.html

data class User(val name: String, val age: Int)
来源：http://hz.hnxiangtu.top/gtviigwkcg.html

[T09] Kotlin：扩展函数
来源：http://hz.zhengqikj.top/gtcwbplzlc.html

fun String.exclaim() = this + "!"
来源：http://hz.52xcode.cn/gtmxwmhwcd.html

[T10] Kotlin：默认参数
来源：http://hz.gogol.net.cn/gtvspsedar.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yvedp.cn/gtjlwqbkhk.html

[T11] Kotlin：协程
来源：http://hz.shzxlz.cn/gtbqbxeayq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ybcxt.top/gtnlipohsq.html

[T12] Kotlin：解构声明
来源：http://hz.ppjwa.cn/gtwmnwamtb.html

val (a, b) = Pair(1, 2)
来源：http://hz.shangyingyoupin.top/gtrqhbqnfy.html

[T13] Kotlin：只读 Map
来源：http://hz.nwbrower.top/gtroarpckc.html

val m = mapOf("a" to 1)
来源：http://hz.xylfe.cn/gtldxrumhg.html

[T14] Kotlin：循环
来源：http://hz.wangshuangyany.cn/gtfwiocnjw.html

for (i in 1..10) println(i)
来源：http://hz.pycfn.com/gtbpaxxxmp.html

[T15] Kotlin：接口
来源：http://hz.ydjk.org.cn/gtdultknww.html

interface Shape { fun area(): Double }
来源：http://hz.nwbrower.top/gtoxsbxvxg.html

[T16] Swift：Hello World
来源：http://hz.bjfxy.top/gtehrfmorr.html

print("Hello")
来源：http://hz.hysaishi.cn/gtbjanxyyl.html

[T17] Swift：变量与常量
来源：http://hz.pengpengdd.cyou/gttohxuxqz.html

var a = 1;  let b = 2
来源：http://hz.yj202588.top/gtozxnsajs.html

[T18] Swift：字符串插值
来源：http://hz.52xcode.cn/gteimuwazl.html

"值: \(b)"
来源：http://hz.jyoumei.cn/gtzwmetkos.html

[T19] Swift：可选绑定
来源：http://hz.9152youxi.cn/gtdoaickpf.html

if let n = opt { print(n) }
来源：http://hz.aizwys.cn/gtquzvmegu.html

[T20] Swift：数组操作
来源：http://hz.svipenyu.cn/gtulqvlpbb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shuidangran.top/gtpsiialck.html

[T21] Swift：遍历
来源：http://hz.sysykeji.top/gtgeqnsgjh.html

for x in a { print(x) }
来源：http://hz.ydzc1.top/gtgvrqvthn.html

[T22] Swift：字典
来源：http://hz.iojbl.cn/gtlbicmkvm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ydzc1.top/gthyelrlsw.html

[T23] Swift：函数
来源：http://hz.fengsongda.top/gtibbevvwq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hfpthk.cn/gtgitbmqho.html

[T24] Swift：闭包
来源：http://hz.c1oappe.top/gtgukkofpf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhengqikj.top/gtrjrroehz.html

[T25] Swift：结构体
来源：http://hz.zhaomingkeji.xyz/gtipflqohl.html

struct P { var x: Int }
来源：http://hz.hnxiangtu.top/gtvtbbbfpm.html

[T26] Swift：类与重写
来源：http://hz.ivvv.top/gtyevrjsui.html

class A: Base { override func f() {} }
来源：http://hz.jianghu66.top/gtaywwavyk.html

[T27] Swift：错误处理
来源：http://hz.hnxiangtu.top/gttsjiguuj.html

do { try f() } catch { print(error) }
来源：http://hz.iojbl.cn/gttlzmrpxp.html

[T28] Swift：枚举
来源：http://hz.zdqjudy.top/gtygeqiuyo.html

enum Color { case red, green }
来源：http://hz.cqqwz.cn/gtabqvnnkp.html

[T29] Swift：guard 提前返回
来源：http://hz.ydzc1.top/gtshivxkzb.html

guard let x = opt else { return }
来源：http://hz.gogol.net.cn/gtemxplrej.html

[T30] Swift：协议
来源：http://hz.cucudq.cn/gtczaylyql.html

protocol Shape { func area() -> Double }
来源：http://hz.nanxinkj.top/gtgwoddkta.html

[T31] Lua：Hello World
来源：http://hz.tian-w.cn/gtbwcverdo.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gtzlzivepv.html

[T32] Lua：局部变量
来源：http://hz.sufxvd.cn/gtxxubrirt.html

local a = 1
来源：http://hz.hnxiangtu.top/gtlpkqvjlx.html

[T33] Lua：表（数组）
来源：http://hz.jianghu66.top/gtvcavsqix.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ppjwa.cn/gtxmwdnqxa.html

[T34] Lua：遍历表
来源：http://hz.zhixingplan.top/gtccyeqktw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.haohaochexian.top/gtjccnrgnf.html

[T35] Lua：字典表
来源：http://hz.sweek.top/gtptosplqc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.meibo888.top/gtfrenyqyf.html

[T36] Lua：函数
来源：http://hz.shzxlz.cn/gtvdglaapr.html

function add(a, b) return a + b end
来源：http://hz.birdmap.top/gtpypbpbdi.html

[T37] Lua：字符串拼接
来源：http://hz.316326.xyz/gtgltkgvrw.html

"a" .. "b"
来源：http://hz.jinqigfzy.top/gtujrowucg.html

[T38] Lua：条件
来源：http://hz.pycfn.com/gtmuluslqz.html

if x > 0 then print("正") end
来源：http://hz.xinyue.icu/gtuarhbfhp.html

[T39] Lua：模式匹配
来源：http://hz.tianlin.xyz/gteuzurcrs.html

string.find(s, "%d+")
来源：http://hz.pengpengdd.cyou/gtalmwyecx.html

[T40] Lua：元表
来源：http://hz.jinghuilouyu.cn/gtolddajnu.html

setmetatable({}, { __index = base })
来源：http://hz.zhoulong.xyz/gtengeeplo.html

[T41] Perl：Hello World
来源：http://hz.tianlin.xyz/gtmwlrraga.html

print "Hello\n";
来源：http://hz.dianchejie.cn/gtwhqtevql.html

[T42] Perl：变量类型
来源：http://hz.shzxlz.cn/gtswrghhnj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.meibo888.top/gtgquryolc.html

[T43] Perl：字符串插值
来源：http://hz.sysykeji.top/gtjzombxiz.html

"值: $a"
来源：http://hz.xingfuxueyuan.xyz/gtvxfnukcm.html

[T44] Perl：条件
来源：http://hz.shangyingyoupin.top/gtjhfohkhm.html

if ($a > 0) { print "正"; }
来源：http://hz.hnxiangtu.top/gtmuojgplg.html

[T45] Perl：数组遍历
来源：http://hz.tian-w.cn/gthgvihhst.html

for my $x (@arr) { print $x; }
来源：http://hz.chenlongwang.top/gtswuqwitk.html

[T46] Perl：哈希操作
来源：http://hz.zdqjudy.top/gtngwzvhla.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sweek.top/gtaucbeegf.html

[T47] Perl：正则捕获
来源：http://hz.feifeiyinyue.top/gtzkrmeasp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.havefunace.top/gthwzvwpmz.html

[T48] Perl：正则替换
来源：http://hz.yj202588.top/gtbvirlqrz.html

$s =~ s/old/new/g;
来源：http://hz.jianghu66.top/gtuhtfukeq.html

[T49] Perl：函数
来源：http://hz.birdmap.top/gtawdoufhn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jiagoushi.top/gtvpmxqnnn.html

[T50] Perl：逐行读文件
来源：http://hz.jianghu66.top/gtxkinbglo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tian-w.cn/gtxlcolmjc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jqgufenzy.top/gtanojjdul.html

[T51] Scala：Hello World
来源：http://hz.yuxming.cn/gtrinqxkay.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gtzbszvhrd.html

[T52] Scala：变量
来源：http://hz.iojbl.cn/gtggpfabuo.html

val a = 1;  var b = 2
来源：http://hz.redwolf501.top/gtpriqczno.html

[T53] Scala：字符串插值
来源：http://hz.andypj.xyz/gtwdbburme.html

s"值: $b"
来源：http://hz.sweek.top/gtckzyyprn.html

[T54] Scala：集合映射
来源：http://hz.52xcode.cn/gtvocrvfbk.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.feifeiyinyue.top/gtyvjxhcxl.html

[T55] Scala：集合过滤
来源：http://hz.shanyushiyangkeji.top/gtgvzssdrm.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jyoumei.cn/gtwbatmnmc.html

[T56] Scala：样例类
来源：http://hz.ybcxt.top/gtfrhzogbc.html

case class User(name: String, age: Int)
来源：http://hz.haohaochexian.top/gthuqlssku.html

[T57] Scala：模式匹配
来源：http://hz.zhengqikj.top/gtzdqaoqkj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.fzhhl.top/gtrbishykc.html

[T58] Scala：函数定义
来源：http://hz.xziqi.cn/gtmvojoyha.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.birdmap.top/gtdqtgjlkv.html

[T59] Scala：循环
来源：http://hz.yueranfly.top/gtiwqaopww.html

for (i <- 1 to 10) println(i)
来源：http://hz.tianlin.xyz/gtzemoiopx.html

[T60] Scala：折叠
来源：http://hz.shangyingyoupin.top/gtifvnoomm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.wangshuangyany.cn/gthudvzdkz.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtalxdzfnv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenzaomai.com/gtamclpehb.html

================================================================================
来源：http://hz.jyoumei.cn/gtdvstzfiy.html

[U01] Py：创建虚拟环境
来源：http://hz.chenzaomai.com/gtjrbxxrly.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hywenlv.cn/gtlceahelo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.meibo888.top/gtnskenkxn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.tanke756.top/gtixuyjzkt.html

[U03] Py：加载 .env 配置
来源：http://hz.sweek.top/gtqsossyug.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.0kj1m.cn/gtjyxjnqxy.html

[U04] Py：变量调试打印
来源：http://hz.smart0.xyz/gtjobnzbis.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xuanzx.com/gtffdrqivb.html

[U05] Py：列表去重且保序
来源：http://hz.yuanzhike.top/gtmqjljizm.html

list(dict.fromkeys(arr))
来源：http://hz.xziqi.cn/gtoiqqnjyj.html

[U06] Py：合并两个字典
来源：http://hz.jinghuilouyu.cn/gtewbwvkuh.html

{**a, **b}
来源：http://hz.gotoacloud.top/gtjnmvivkr.html

[U07] Py：反转字典键值
来源：http://hz.cheryme.top/gtgzcusudg.html

{v: k for k, v in d.items()}
来源：http://hz.sufxvd.cn/gtotcmvnzn.html

[U08] Py：展平二维列表
来源：http://hz.shangyingyoupin.top/gthmhfxlsd.html

[y for x in nested for y in x]
来源：http://hz.ywan-chungtsiang.top/gtfbhnrjgw.html

[U09] Py：字典取最大值的键
来源：http://hz.ybcxt.top/gtkusiiorm.html

max(d, key=d.get)
来源：http://hz.jqgufenzy.top/gtgenouven.html

[U10] Py：按值排序字典
来源：http://hz.shanyushiyangtech.top/gtkctjxmor.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ydzc1.top/gtnznbxtpv.html

[U11] Py：生成器表达式
来源：http://hz.vqdsnc.cn/gtglzjtonj.html

(x * 2 for x in arr)
来源：http://hz.hammf.cn/gtgdbcbaly.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tanke756.top/gtehykufra.html

Counter(arr).most_common(3)
来源：http://hz.zdqjudy.top/gtibujwfiv.html

[U13] Py：固定长度队列
来源：http://hz.cucudq.cn/gtgduuakgi.html

deque(maxlen=10)
来源：http://hz.hysaishi.cn/gtltsgabul.html

[U14] Py：分组收集到列表
来源：http://hz.shangyingyoupin.top/gtlfrvnvtd.html

defaultdict(list)
来源：http://hz.yuanzhike.top/gtlujyqxbr.html

[U15] Py：高精度计时
来源：http://hz.yj202588.top/gthnkqxjjc.html

t = time.perf_counter()
来源：http://hz.nwbrower.top/gtjtnorwvc.html

[U16] Py：命令行参数解析
来源：http://hz.xingfuxueyuan.xyz/gtmdjwzrfc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.havefunace.top/gtjwzpkbai.html

[U17] Py：初始化日志
来源：http://hz.cucudq.cn/gtlflshxkb.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yongpay.top/gtywjuoshu.html

[U18] Py：预编译正则
来源：http://hz.yangfankeji.com/gtsavoxsjz.html

pat = re.compile(r"\d+")
来源：http://hz.cashguo.top/gthcqexupd.html

[U19] Py：正则替换带回调
来源：http://hz.tianlin.xyz/gtqitfoxpp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hysaishi.cn/gtnkmingir.html

[U20] Py：缓存函数结果
来源：http://hz.yj202588.top/gtdjvdvczc.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hfpthk.cn/gtobzptfdo.html

[U21] Py：自定义上下文管理器
来源：http://hz.cucudq.cn/gttvcqrkkc.html

@contextlib.contextmanager
来源：http://hz.dashuyun.cn/gtjvrkupds.html

[U22] Py：矩阵转置
来源：http://hz.jyoumei.cn/gthzzmsfbm.html

list(zip(*m))
来源：http://hz.jqgufenzy.top/gtaydhexbq.html

[U23] Py：分块读取大文件
来源：http://hz.jinyuanbaomall.cn/gtzzqsxcec.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.havefunace.top/gthcrykexr.html

[U24] Py：路径操作
来源：http://hz.aibaodan.cn/gtskvfpokk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhaomingkeji.xyz/gtbrdvyhrt.html

[U25] Py：CSV 按字典读
来源：http://hz.yuanzhike.top/gtxwgmejbt.html

csv.DictReader(f)
来源：http://hz.hfpthk.cn/gtnfpxzrew.html

[U26] Py：并发下载
来源：http://hz.pengpengdd.cyou/gththfbgnu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhengqikj.top/gtrvbhhxsk.html

[U27] Py：异步 HTTP
来源：http://hz.sufxvd.cn/gthodcqxwr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.0kj1m.cn/gtnosrlglc.html

[U28] Py：类型别名
来源：http://hz.daxiang520.top/gtlhacehlg.html

UserId = int
来源：http://hz.xinyue.icu/gtbrffxopr.html

[U29] Py：属性校验
来源：http://hz.ehwqpu.com/gtfxfnmizv.html

@property 与 @x.setter 配合
来源：http://hz.jinyuanbaomall.cn/gtvdsvkwdp.html

[U30] Py：数据类
来源：http://hz.fengsongda.top/gtvrxamtlm.html

@dataclass(slots=True)
来源：http://hz.hongshengwenyu.top/gtmztkyqcd.html

[U31] Py：单测
来源：http://hz.xingfuxueyuan.xyz/gtwaqjocrd.html

python -m pytest -q
来源：http://hz.cdnleiting.top/gtcwujisqa.html

[U32] Py：代码格式化
来源：http://hz.wangshuangyany.cn/gttertkbae.html

ruff format . && ruff check --fix .
来源：http://hz.jqgfzy.top/gtrsbfxszk.html

[U33] Py：打包发布
来源：http://hz.yvedp.cn/gtodmkancd.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ivvv.top/gtbeupxnye.html

[U34] Py：判断编码
来源：http://hz.yj202588.top/gtruucmagy.html

chardet.detect(raw)
来源：http://hz.yuxming.cn/gtaewpgoni.html

[U35] Py：发送邮件
来源：http://hz.xuanzx.com/gtqmrhmeac.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hammf.cn/gtdsehdafm.html

[U36] Py：定时任务
来源：http://hz.gzhubu.top/gtcqciwoqe.html

schedule.every(10).minutes.do(job)
来源：http://hz.jianghu66.top/gtynpumkwy.html

[U37] Py：读写 Excel
来源：http://hz.fengsongda.top/gtvzexclno.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jianghu66.top/gthdelaolp.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhixingplan.top/gttjtkohny.html

Path(__file__).resolve().parent
来源：http://hz.vqdsnc.cn/gtbyeehspg.html

[U39] Py：判断是否在交互环境
来源：http://hz.haohaochexian.top/gtoefysxrw.html

sys.stdout.isatty()
来源：http://hz.jlsjyb.cn/gtyrzmyswh.html

[U40] Py：打印到标准错误
来源：http://hz.jinghuilouyu.cn/gtfckbqlnq.html

print("err", file=sys.stderr)
来源：http://hz.zhiwuduotai.top/gtwqwysdyg.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.tian-w.cn/gtwvnhkfdr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.birdmap.top/gtvoezyhci.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sufxvd.cn/gtkdvtmbgr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinghuilouyu.cn/gtkgyptyyw.html

[U43] PHP：声明命名空间
来源：http://hz.hywenlv.cn/gtutedlgji.html

namespace App\Http;
来源：http://hz.hnqzz.top/gtebvsuvmj.html

[U44] PHP：开启严格类型
来源：http://hz.jianghu66.top/gttbmvsrvh.html

declare(strict_types=1);
来源：http://hz.ppjwa.cn/gtmfmofxda.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shanyushiyangkeji.top/gtynskwpkw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gtcqrrjwuf.html

[U46] PHP：可空类型
来源：http://hz.wangdashe.top/gtfqbkruqn.html

?string $name = null
来源：http://hz.cucudq.cn/gtwhbkmvro.html

[U47] PHP：联合类型
来源：http://hz.meibo888.top/gtppogdzoo.html

int|string $id
来源：http://hz.haohaochexian.top/gtzadksyhc.html

[U48] PHP：纯枚举
来源：http://hz.ivvv.top/gtdlamyhep.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gaohongyu789.top/gtyirzwnuh.html

[U49] PHP：只读属性
来源：http://hz.daxiang520.top/gtkzhoxhpt.html

public readonly string $name
来源：http://hz.hysaishi.cn/gtpioluvso.html

[U50] PHP：构造器属性提升
来源：http://hz.cqqwz.cn/gtujnbvguf.html

public function __construct(private int $id) {}
来源：http://hz.tianlin.xyz/gtqtxwvdkw.html

[U51] PHP：数组解构
来源：http://hz.bjfxy.top/gtghflmykr.html

[$a, $b] = $arr;
来源：http://hz.daxiang520.top/gtbmedvdye.html

[U52] PHP：箭头函数
来源：http://hz.xinyue.icu/gtmfrafjfn.html

$double = fn($x) => $x * 2;
来源：http://hz.hysaishi.cn/gtuxgnoywe.html

[U53] PHP：空合并运算符
来源：http://hz.shanyushiyangtech.top/gtvvmeeapv.html

$v = $a ?? $b ?? "default";
来源：http://hz.shangyingyoupin.top/gtszbjyfxq.html

[U54] PHP：空安全调用
来源：http://hz.jiagoushi.top/gtxguhanjh.html

$obj?->method()
来源：http://hz.dashuyun.cn/gtgbdvwfeb.html

[U55] PHP：match 表达式
来源：http://hz.zdqjudy.top/gtcefweocz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.tanke756.top/gtqtgermyo.html

[U56] PHP：命名参数
来源：http://hz.xziqi.cn/gtpsssjfez.html

f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtthjohmdh.html

[U57] PHP：字符串插值
来源：http://hz.daria6918.cn/gtvsnuyllv.html

"值: {$a}"
来源：http://hz.haohaochexian.top/gtdxwqksdz.html

[U58] PHP：数组三件套
来源：http://hz.vqdsnc.cn/gtmnrgacha.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinyuanbaomall.cn/gtztuciwul.html

[U59] PHP：自定义排序
来源：http://hz.shanyushiyangtech.top/gtufuiwris.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ywan-chungtsiang.top/gtchnqgvpm.html

[U60] PHP：JSON 编解码
来源：http://hz.aibaodan.cn/gtftolvobp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ydjk.org.cn/gtyjxspkic.html

[U61] PHP：正则
来源：http://hz.feifeiyinyue.top/gtmgeqcvac.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhongyouzk.top/gtalmrblye.html

[U62] PHP：日期对象
来源：http://hz.hongshengwenyu.top/gtoqmqbzpn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ywan-chungtsiang.top/gtmayczegy.html

[U63] PHP：文件读写
来源：http://hz.hongshengwenyu.top/gtobnmgqjb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jqgufenzy.top/gtsbrxtsor.html

[U64] PHP：目录遍历
来源：http://hz.haohaochexian.top/gtsrvrpsxf.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.andypj.xyz/gtkmaidfty.html

[U65] PHP：会话
来源：http://hz.fzhhl.top/gtkmxdtbdc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yj20258.top/gtxkwtshbo.html

[U66] PHP：设置 Cookie
来源：http://hz.chenlongwang.top/gtzvezzgtr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhoulong.xyz/gttxiieckx.html

[U67] PHP：处理文件上传
来源：http://hz.iojbl.cn/gtrggxewnp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.bjfxy.top/gtwmcjrdbe.html

[U68] PHP：PDO 连接
来源：http://hz.jyoumei.cn/gtoajnxnbk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.fzhhl.top/gtriqpcmzr.html

[U69] PHP：PDO 预处理
来源：http://hz.gogol.net.cn/gtyqryozfl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.meibo888.top/gtamkmnxpi.html

[U70] PHP：PDO 事务
来源：http://hz.yangfankeji.com/gtlrgnkkkk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.sweek.top/gtxhlmpwkh.html

[U71] PHP：抛出异常
来源：http://hz.yvedp.cn/gtuzdozfqc.html

throw new RuntimeException("失败", 500);
来源：http://hz.jqgfzy.top/gtjnnfemnx.html

[U72] PHP：写错误日志
来源：http://hz.redwolf501.top/gthkivwrlr.html

error_log("失败: " . $e->getMessage());
来源：http://hz.quarkkingdee.top/gtmjxmtrli.html

[U73] PHP：读取 ini 配置
来源：http://hz.andypj.xyz/gtqbvgwsvu.html

parse_ini_file("config.ini", true)
来源：http://hz.hysaishi.cn/gttyhuvarv.html

[U74] PHP：读取环境变量
来源：http://hz.gogol.net.cn/gtwmakphhg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.bjfxy.top/gtezcpzzmt.html

[U75] PHP：依赖注入
来源：http://hz.gzhubu.top/gtlutiwiue.html

composer require psr/container
来源：http://hz.smart0.xyz/gtrqyynixv.html

[U76] PHP：简单路由
来源：http://hz.jinqigufen.top/gtmesumqyd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.cashguo.top/gtbpuypjmt.html

[U77] PHP：模板渲染
来源：http://hz.cqqwz.cn/gtmehegzsr.html

composer require twig/twig
来源：http://hz.ivvv.top/gtwsnbiyim.html

[U78] PHP：单元测试
来源：http://hz.andypj.xyz/gtjosyajdp.html

composer require --dev phpunit/phpunit
来源：http://hz.9152youxi.cn/gtbvzikfnw.html

[U79] PHP：静态分析
来源：http://hz.nwbrower.top/gtpxuhitpl.html

composer require --dev phpstan/phpstan
来源：http://hz.cashguo.top/gtjwgbwjhv.html

[U80] PHP：代码规范修复
来源：http://hz.haohaochexian.top/gtylceaumh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.shangyingyoupin.top/gtczjuujin.html

[U81] JS：初始化项目
来源：http://hz.yvedp.cn/gtdrvtegtn.html

npm init -y;  npm i express
来源：http://hz.snrcjt.cn/gtlbnabukt.html

[U82] JS：package.json 脚本
来源：http://hz.mhx1999.top/gtqrunxwut.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.birdmap.top/gtqhmgqcjp.html

[U83] JS：ES Module 导入导出
来源：http://hz.hongshengwenyu.top/gtcfyuyhwf.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhaomingkeji.xyz/gtjmeylkep.html

[U84] JS：CommonJS 写法
来源：http://hz.guowangkeji.top/gtbbxshedx.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zhongyouzk.top/gtjpxayuco.html


<!-- 参考信息 -->