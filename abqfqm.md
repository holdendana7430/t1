代发 wailian999

[T01] Kotlin：Hello World
来源：http://hz.zhengqikj.top/gtzfgfyvak.html

println("Hello")
来源：http://hz.yj20258.top/gtozdmrqoi.html

[T02] Kotlin：变量
来源：http://hz.quarkkingdee.top/gtwahiodsa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yuxming.cn/gtuflhzwqo.html

[T03] Kotlin：字符串模板
来源：http://hz.xingfuxueyuan.xyz/gtuiyxmywd.html

"值: $b"
来源：http://hz.fzhhl.top/gtrssduckp.html

[T04] Kotlin：空安全
来源：http://hz.tianlin.xyz/gtanihyair.html

val n: String? = null;  n?.length
来源：http://hz.pengpengdd.cyou/gtgojquzto.html

[T05] Kotlin：when 表达式
来源：http://hz.wangdashe.top/gtqoowrftr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.pengpengdd.cyou/gtujmeapmu.html

[T06] Kotlin：集合映射
来源：http://hz.zhixingplan.top/gtfvmsrwuq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hywenlv.cn/gteodqohrr.html

[T07] Kotlin：集合过滤
来源：http://hz.yongpay.top/gtsvgskdmb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.iojbl.cn/gtuyygmomn.html

[T08] Kotlin：数据类
来源：http://hz.fzhhl.top/gtpndjrfsj.html

data class User(val name: String, val age: Int)
来源：http://hz.tianlin.xyz/gtacgqsmof.html

[T09] Kotlin：扩展函数
来源：http://hz.zhixingplan.top/gtdnsomqzv.html

fun String.exclaim() = this + "!"
来源：http://hz.xziqi.cn/gttbylxhxs.html

[T10] Kotlin：默认参数
来源：http://hz.shanyushiyangkeji.top/gtxmwzqgum.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinyuanbaomall.cn/gtrsbfwlsz.html

[T11] Kotlin：协程
来源：http://hz.guannengcc.top/gtrhmafkgi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinyuanbaomall.cn/gtexbspbbu.html

[T12] Kotlin：解构声明
来源：http://hz.tanke756.top/gtpwuqkyxm.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhongyouzk.top/gtabyceirp.html

[T13] Kotlin：只读 Map
来源：http://hz.nanxinkj.top/gtaeedmvvi.html

val m = mapOf("a" to 1)
来源：http://hz.ivvv.top/gtnvdhhbny.html

[T14] Kotlin：循环
来源：http://hz.shzxlz.cn/gtotdmnvvo.html

for (i in 1..10) println(i)
来源：http://hz.haohaochexian.top/gtfpuznedx.html

[T15] Kotlin：接口
来源：http://hz.guannengcc.top/gtmahgccxw.html

interface Shape { fun area(): Double }
来源：http://hz.sysykeji.top/gtxodmaxry.html

[T16] Swift：Hello World
来源：http://hz.ydjk.org.cn/gtyctvagta.html

print("Hello")
来源：http://hz.yj20258.top/gtfxkwjslj.html

[T17] Swift：变量与常量
来源：http://hz.vqdsnc.cn/gtxxylgeco.html

var a = 1;  let b = 2
来源：http://hz.cucudq.cn/gttnksvgyi.html

[T18] Swift：字符串插值
来源：http://hz.jianghu66.top/gtkcjerqtx.html

"值: \(b)"
来源：http://hz.shanyushiyangkeji.top/gtzmqwgvyk.html

[T19] Swift：可选绑定
来源：http://hz.nwbrower.top/gtsuopfvfj.html

if let n = opt { print(n) }
来源：http://hz.redwolf501.top/gtkvigwtja.html

[T20] Swift：数组操作
来源：http://hz.hnqzz.top/gtlwrpepqy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jyoumei.cn/gtabxfvxwl.html

[T21] Swift：遍历
来源：http://hz.hysaishi.cn/gtdiakkgkl.html

for x in a { print(x) }
来源：http://hz.zhengqikj.top/gtkbatcegq.html

[T22] Swift：字典
来源：http://hz.ivvv.top/gtniqovyeg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ywan-chungtsiang.top/gtrvybxyoo.html

[T23] Swift：函数
来源：http://hz.zhongyouzk.top/gtiwptbkyc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hnxiangtu.top/gtssgzhmqp.html

[T24] Swift：闭包
来源：http://hz.guowangkeji.top/gtlecehlmh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenzaomai.com/gtlwdmrjqy.html

[T25] Swift：结构体
来源：http://hz.feifeiyinyue.top/gtyipemfxu.html

struct P { var x: Int }
来源：http://hz.hfpthk.cn/gtlroippub.html

[T26] Swift：类与重写
来源：http://hz.xingfuxueyuan.xyz/gtqcntnahn.html

class A: Base { override func f() {} }
来源：http://hz.nwbrower.top/gtporlxufd.html

[T27] Swift：错误处理
来源：http://hz.shuidangran.top/gtarughwmb.html

do { try f() } catch { print(error) }
来源：http://hz.tanke756.top/gtwknhmkwb.html

[T28] Swift：枚举
来源：http://hz.jinghuilouyu.cn/gtjstliroq.html

enum Color { case red, green }
来源：http://hz.zycfv.cn/gtsybdlwhr.html

[T29] Swift：guard 提前返回
来源：http://hz.redwolf501.top/gtshdzrtit.html

guard let x = opt else { return }
来源：http://hz.iojbl.cn/gtussarryz.html

[T30] Swift：协议
来源：http://hz.mhx1999.top/gtooruucjk.html

protocol Shape { func area() -> Double }
来源：http://hz.ybcxt.top/gtfksgucur.html

[T31] Lua：Hello World
来源：http://hz.zdqjudy.top/gthsgfksgq.html

print("Hello")
来源：http://hz.yongpay.top/gtiyoyfnqa.html

[T32] Lua：局部变量
来源：http://hz.hammf.cn/gtmptxqjph.html

local a = 1
来源：http://hz.ydjk.org.cn/gtblsbhfqq.html

[T33] Lua：表（数组）
来源：http://hz.0kj1m.cn/gtvyqdhpiq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangshuangyany.cn/gtxcmyayao.html

[T34] Lua：遍历表
来源：http://hz.andypj.xyz/gtgowwrkjc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.c1oappe.top/gtiducjrmr.html

[T35] Lua：字典表
来源：http://hz.hongshengwenyu.top/gtmgigeiom.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xziqi.cn/gtbzdzlwbl.html

[T36] Lua：函数
来源：http://hz.zhengqikj.top/gtqkknkwmx.html

function add(a, b) return a + b end
来源：http://hz.kuanghao11.cn/gtkynvxwea.html

[T37] Lua：字符串拼接
来源：http://hz.jinqigufen.top/gtoywztydp.html

"a" .. "b"
来源：http://hz.snrcjt.cn/gtvqmjkjyb.html

[T38] Lua：条件
来源：http://hz.hfpthk.cn/gtznxapauj.html

if x > 0 then print("正") end
来源：http://hz.xuetiantiany.cn/gtlzqqthul.html

[T39] Lua：模式匹配
来源：http://hz.jqgfzy.top/gtogelvdyt.html

string.find(s, "%d+")
来源：http://hz.jiagoushi.top/gtbpdbnmgy.html

[T40] Lua：元表
来源：http://hz.yj202588.top/gtidfybxuj.html

setmetatable({}, { __index = base })
来源：http://hz.meibo888.top/gtvorxoziu.html

[T41] Perl：Hello World
来源：http://hz.cashguo.top/gtpnbcnbzs.html

print "Hello\n";
来源：http://hz.jyoumei.cn/gtdmwecelp.html

[T42] Perl：变量类型
来源：http://hz.zycfv.cn/gtmdumtefr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinghuilouyu.cn/gtegzfumaj.html

[T43] Perl：字符串插值
来源：http://hz.0kj1m.cn/gtazxfcymw.html

"值: $a"
来源：http://hz.9152youxi.cn/gtvokwahsv.html

[T44] Perl：条件
来源：http://hz.gotoacloud.top/gtsuclrpfh.html

if ($a > 0) { print "正"; }
来源：http://hz.yanxiufei.cn/gttflwvizi.html

[T45] Perl：数组遍历
来源：http://hz.jlsjyb.cn/gtytvqdvin.html

for my $x (@arr) { print $x; }
来源：http://hz.yj202588.top/gtysqofhco.html

[T46] Perl：哈希操作
来源：http://hz.9152youxi.cn/gtcytwwukv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gaohongyu789.top/gtacfxmsah.html

[T47] Perl：正则捕获
来源：http://hz.gaohongyu789.top/gtkzwsjemj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yonumen.top/gtoypxicay.html

[T48] Perl：正则替换
来源：http://hz.0kj1m.cn/gtnzlldfkj.html

$s =~ s/old/new/g;
来源：http://hz.sysykeji.top/gtnzgmdfoi.html

[T49] Perl：函数
来源：http://hz.daxiang520.top/gtnokpykgr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.meibo888.top/gtxfbdoxtf.html

[T50] Perl：逐行读文件
来源：http://hz.aibaodan.cn/gtygvzoixr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yuxming.cn/gtbukhsmrz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.dashuyun.cn/gthudouwaf.html

[T51] Scala：Hello World
来源：http://hz.hnqzz.top/gtdynsykcq.html

println("Hello")
来源：http://hz.52xcode.cn/gtjpnaxibx.html

[T52] Scala：变量
来源：http://hz.gzhubu.top/gtietfwhat.html

val a = 1;  var b = 2
来源：http://hz.chenzaomai.com/gtabaninxv.html

[T53] Scala：字符串插值
来源：http://hz.hysaishi.cn/gtjydtosve.html

s"值: $b"
来源：http://hz.ehwqpu.com/gtpkhrxuxn.html

[T54] Scala：集合映射
来源：http://hz.zhongyouzk.top/gtbphtylri.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.redwolf501.top/gtrijbylkq.html

[T55] Scala：集合过滤
来源：http://hz.cheryme.top/gtrsrhwxtc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.aizwys.cn/gtnizpfbud.html

[T56] Scala：样例类
来源：http://hz.yanxiufei.cn/gtcntlywmc.html

case class User(name: String, age: Int)
来源：http://hz.hongshengwenyu.top/gtkialbfqx.html

[T57] Scala：模式匹配
来源：http://hz.zhijiandao.cn/gtegysbfkb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shzxlz.cn/gtpsaypcbn.html

[T58] Scala：函数定义
来源：http://hz.shanyushiyangtech.top/gtjmcthemc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xinyue.icu/gtqvsrsdcx.html

[T59] Scala：循环
来源：http://hz.jqgufenzy.top/gtmhfzhmci.html

for (i <- 1 to 10) println(i)
来源：http://hz.c1oappe.top/gtavpbvtbb.html

[T60] Scala：折叠
来源：http://hz.hongshengwenyu.top/gtajioupfs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.nanxinkj.top/gtccqbktuw.html

================================================================================
来源：http://hz.mhx1999.top/gtzlpuneyv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhongyouzk.top/gtlhpviwog.html

================================================================================
来源：http://hz.jinqigfzy.top/gtpvieeotg.html

[U01] Py：创建虚拟环境
来源：http://hz.ywan-chungtsiang.top/gtpweuviqa.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tianlin.xyz/gtoirwmcwp.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cheryme.top/gtjvogmrlf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.andypj.xyz/gtadndgxcp.html

[U03] Py：加载 .env 配置
来源：http://hz.zdqjudy.top/gtxzwqhyfn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhaomingkeji.xyz/gtaoucrflv.html

[U04] Py：变量调试打印
来源：http://hz.jinqigufen.top/gtnovtqpsx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinqigufen.top/gtoswvyndq.html

[U05] Py：列表去重且保序
来源：http://hz.ivvv.top/gtefytwefz.html

list(dict.fromkeys(arr))
来源：http://hz.shzxlz.cn/gtkfdinqpk.html

[U06] Py：合并两个字典
来源：http://hz.hfpthk.cn/gtkytmjqik.html

{**a, **b}
来源：http://hz.zycfv.cn/gtfgzerwig.html

[U07] Py：反转字典键值
来源：http://hz.yongpay.top/gtnbalwjsa.html

{v: k for k, v in d.items()}
来源：http://hz.zdqjudy.top/gtfaahgbci.html

[U08] Py：展平二维列表
来源：http://hz.smart0.xyz/gtafngwfyj.html

[y for x in nested for y in x]
来源：http://hz.hfpthk.cn/gtthswqmrw.html

[U09] Py：字典取最大值的键
来源：http://hz.shanyushiyangtech.top/gtqupzwmmh.html

max(d, key=d.get)
来源：http://hz.vqdsnc.cn/gthfkvtxxp.html

[U10] Py：按值排序字典
来源：http://hz.zhiwuduotai.top/gtmvnwcohv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gzhubu.top/gtsvtxgpuu.html

[U11] Py：生成器表达式
来源：http://hz.shanyushiyangkeji.top/gtnsqseodm.html

(x * 2 for x in arr)
来源：http://hz.shzxlz.cn/gtbxdjsadr.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yangfankeji.com/gtozoxnflf.html

Counter(arr).most_common(3)
来源：http://hz.hywenlv.cn/gtubqudmdr.html

[U13] Py：固定长度队列
来源：http://hz.sxryk.cn/gtphetswzg.html

deque(maxlen=10)
来源：http://hz.pengpengdd.cyou/gtypeexzxv.html

[U14] Py：分组收集到列表
来源：http://hz.pycfn.com/gtolvimwum.html

defaultdict(list)
来源：http://hz.nanxuanxn.top/gtakmmpblq.html

[U15] Py：高精度计时
来源：http://hz.smart0.xyz/gtougcypsz.html

t = time.perf_counter()
来源：http://hz.dianchejie.cn/gteehfocto.html

[U16] Py：命令行参数解析
来源：http://hz.jyoumei.cn/gtgpcspprs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nwbrower.top/gtmyindpfd.html

[U17] Py：初始化日志
来源：http://hz.ppjwa.cn/gtkmizqgee.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.andypj.xyz/gtcuimjoht.html

[U18] Py：预编译正则
来源：http://hz.gogol.net.cn/gtljrkvdto.html

pat = re.compile(r"\d+")
来源：http://hz.daxiang520.top/gtvjbshvhg.html

[U19] Py：正则替换带回调
来源：http://hz.iojbl.cn/gtoxvwtsrt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.gogol.net.cn/gtrxaitplm.html

[U20] Py：缓存函数结果
来源：http://hz.jyoumei.cn/gtzeimcfef.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jiagoushi.top/gtacaqaeww.html

[U21] Py：自定义上下文管理器
来源：http://hz.hysaishi.cn/gtpkghicmk.html

@contextlib.contextmanager
来源：http://hz.jinyuanbaomall.cn/gtorcfkitp.html

[U22] Py：矩阵转置
来源：http://hz.jinyuanbaomall.cn/gtrwknusvl.html

list(zip(*m))
来源：http://hz.zhijiandao.cn/gteytvxjwo.html

[U23] Py：分块读取大文件
来源：http://hz.xuetiantiany.cn/gthkfmrorh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ivvv.top/gteamwwwmd.html

[U24] Py：路径操作
来源：http://hz.ehwqpu.com/gturqspgsf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhiwuduotai.top/gtousmulgl.html

[U25] Py：CSV 按字典读
来源：http://hz.gaohongyu789.top/gtvywuppkj.html

csv.DictReader(f)
来源：http://hz.gzhubu.top/gtreaizsae.html

[U26] Py：并发下载
来源：http://hz.shanyushiyangtech.top/gtqpiqjucz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.havefunace.top/gtcioksmhp.html

[U27] Py：异步 HTTP
来源：http://hz.jinyuanbaomall.cn/gtewmsxvex.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xinyue.icu/gtoxexcyar.html

[U28] Py：类型别名
来源：http://hz.xylfe.cn/gtmvdxvmrm.html

UserId = int
来源：http://hz.gaohongyu789.top/gtmbqydjot.html

[U29] Py：属性校验
来源：http://hz.hywenlv.cn/gtzlnhjnpg.html

@property 与 @x.setter 配合
来源：http://hz.wangdashe.top/gtivkxcqpe.html

[U30] Py：数据类
来源：http://hz.ehwqpu.com/gtsugigxdt.html

@dataclass(slots=True)
来源：http://hz.zhongyouzk.top/gttagdzikx.html

[U31] Py：单测
来源：http://hz.xinyue.icu/gtcqzkbncl.html

python -m pytest -q
来源：http://hz.sufxvd.cn/gtgbhvuivs.html

[U32] Py：代码格式化
来源：http://hz.chenzaomai.com/gttlywdfkk.html

ruff format . && ruff check --fix .
来源：http://hz.jiagoushi.top/gtxlhzwdpe.html

[U33] Py：打包发布
来源：http://hz.xylfe.cn/gtwryuewsx.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.guowangkeji.top/gtvinveoie.html

[U34] Py：判断编码
来源：http://hz.xziqi.cn/gtidaqrzyo.html

chardet.detect(raw)
来源：http://hz.snrcjt.cn/gteahwlibl.html

[U35] Py：发送邮件
来源：http://hz.yj202588.top/gtxjmbvuks.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.iojbl.cn/gtcygigiya.html

[U36] Py：定时任务
来源：http://hz.gaohongyu789.top/gtmjymxwva.html

schedule.every(10).minutes.do(job)
来源：http://hz.zycfv.cn/gtrjelepek.html

[U37] Py：读写 Excel
来源：http://hz.xuanzx.com/gtudjhzuhi.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xuetiantiany.cn/gthtdnkaia.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhixingplan.top/gtniqimsgf.html

Path(__file__).resolve().parent
来源：http://hz.hfpthk.cn/gttgnzegvo.html

[U39] Py：判断是否在交互环境
来源：http://hz.jqgufenzy.top/gtocrxuipu.html

sys.stdout.isatty()
来源：http://hz.jqgufenzy.top/gtjjjgekcb.html

[U40] Py：打印到标准错误
来源：http://hz.9152youxi.cn/gtiawlcrlf.html

print("err", file=sys.stderr)
来源：http://hz.cqqwz.cn/gtzsmgzjqr.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yuxming.cn/gtvaexbubo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhijiandao.cn/gtwltczsjo.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yangfankeji.com/gtxaxctdbx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yvedp.cn/gtnwxbqnot.html

[U43] PHP：声明命名空间
来源：http://hz.52xcode.cn/gtghbjclen.html

namespace App\Http;
来源：http://hz.jinqigufen.top/gtekwrmofu.html

[U44] PHP：开启严格类型
来源：http://hz.zhixingplan.top/gtvvhttknx.html

declare(strict_types=1);
来源：http://hz.kuanghao11.cn/gtombhjkbq.html

[U45] PHP：类型声明与返回类型
来源：http://hz.tianlin.xyz/gtuxquegka.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtqzccwevl.html

[U46] PHP：可空类型
来源：http://hz.jinghuilouyu.cn/gtnrququkk.html

?string $name = null
来源：http://hz.fengsongda.top/gtwqvwrlyo.html

[U47] PHP：联合类型
来源：http://hz.bjfxy.top/gtcefmuhks.html

int|string $id
来源：http://hz.pycfn.com/gtihtlqyst.html

[U48] PHP：纯枚举
来源：http://hz.yangfankeji.com/gtkmzumfyv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinqigufen.top/gteoxwdayk.html

[U49] PHP：只读属性
来源：http://hz.cucudq.cn/gtebunzjjo.html

public readonly string $name
来源：http://hz.zhaomingkeji.xyz/gtaddgmdyh.html

[U50] PHP：构造器属性提升
来源：http://hz.52xcode.cn/gtcvzsxqhx.html

public function __construct(private int $id) {}
来源：http://hz.hnxiangtu.top/gttzdypzpm.html

[U51] PHP：数组解构
来源：http://hz.gotoacloud.top/gtmgcdpafv.html

[$a, $b] = $arr;
来源：http://hz.yongpay.top/gtttfsdthf.html

[U52] PHP：箭头函数
来源：http://hz.shanyushiyangkeji.top/gtisqogrps.html

$double = fn($x) => $x * 2;
来源：http://hz.nanxuanxn.top/gtfgkreikh.html

[U53] PHP：空合并运算符
来源：http://hz.mhx1999.top/gtkkdyjrkg.html

$v = $a ?? $b ?? "default";
来源：http://hz.pengpengdd.cyou/gtuvlcxuyh.html

[U54] PHP：空安全调用
来源：http://hz.ehwqpu.com/gtndcgpwpt.html

$obj?->method()
来源：http://hz.hongshengwenyu.top/gttpirnrzm.html

[U55] PHP：match 表达式
来源：http://hz.yuanzhike.top/gtxmvvcrgm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cdnleiting.top/gtidyyirmd.html

[U56] PHP：命名参数
来源：http://hz.ehwqpu.com/gtyjmjslnd.html

f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gtfpnjrfwe.html

[U57] PHP：字符串插值
来源：http://hz.gogol.net.cn/gtwhbtzmxw.html

"值: {$a}"
来源：http://hz.tianlin.xyz/gtovbekykt.html

[U58] PHP：数组三件套
来源：http://hz.vqdsnc.cn/gtynfuodvd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinqigfzy.top/gtcpcsynzv.html

[U59] PHP：自定义排序
来源：http://hz.yonumen.top/gtxfmvrifw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.redwolf501.top/gtwxahobci.html

[U60] PHP：JSON 编解码
来源：http://hz.jlsjyb.cn/gthksnmsmc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.dianchejie.cn/gtejajnoci.html

[U61] PHP：正则
来源：http://hz.0kj1m.cn/gtgfemwiyn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ehwqpu.com/gtrtbhhbqp.html

[U62] PHP：日期对象
来源：http://hz.haohaochexian.top/gtoupfwest.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhiwuduotai.top/gtromzbrne.html

[U63] PHP：文件读写
来源：http://hz.hongshengwenyu.top/gtuqkbudbo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.fzhhl.top/gtopbtjkhf.html

[U64] PHP：目录遍历
来源：http://hz.gaohongyu789.top/gtgjtqbnyd.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ydjk.org.cn/gtvguskiii.html

[U65] PHP：会话
来源：http://hz.mhx1999.top/gtlhcbjaha.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yuanzhike.top/gtoffubwcx.html

[U66] PHP：设置 Cookie
来源：http://hz.aizwys.cn/gtxxhzhpif.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.tanke756.top/gtnmoqygcb.html

[U67] PHP：处理文件上传
来源：http://hz.tianlin.xyz/gttvfknxji.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jinyuanbaomall.cn/gttiwhfdsh.html

[U68] PHP：PDO 连接
来源：http://hz.mhx1999.top/gtozoyblnc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shanyushiyangtech.top/gtozyifcks.html

[U69] PHP：PDO 预处理
来源：http://hz.redwolf501.top/gtdtmptkgp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xinyue.icu/gtgurgrjfx.html

[U70] PHP：PDO 事务
来源：http://hz.cheryme.top/gtawdbohkr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.aibaodan.cn/gtgfrxrwga.html

[U71] PHP：抛出异常
来源：http://hz.316326.xyz/gtefiydhvo.html

throw new RuntimeException("失败", 500);
来源：http://hz.yueranfly.top/gtrxebnqfv.html

[U72] PHP：写错误日志
来源：http://hz.nanxinkj.top/gtdlnptdvl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.9152youxi.cn/gtoubgznhd.html

[U73] PHP：读取 ini 配置
来源：http://hz.ywan-chungtsiang.top/gtceocbame.html

parse_ini_file("config.ini", true)
来源：http://hz.hysaishi.cn/gtzziliund.html

[U74] PHP：读取环境变量
来源：http://hz.shanyushiyangtech.top/gtscvzirhy.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhiwuduotai.top/gttduuiznv.html

[U75] PHP：依赖注入
来源：http://hz.jinghuilouyu.cn/gtwfbdjabc.html

composer require psr/container
来源：http://hz.hfpthk.cn/gtbkiobuhq.html

[U76] PHP：简单路由
来源：http://hz.mhx1999.top/gtkztfzjjs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.quarkkingdee.top/gthlypjjar.html

[U77] PHP：模板渲染
来源：http://hz.fengsongda.top/gtmdisfalz.html

composer require twig/twig
来源：http://hz.birdmap.top/gtapakwfvo.html

[U78] PHP：单元测试
来源：http://hz.mhx1999.top/gtpxqztwyw.html

composer require --dev phpunit/phpunit
来源：http://hz.316326.xyz/gtyqoplnlx.html

[U79] PHP：静态分析
来源：http://hz.shzxlz.cn/gtjwqxoepa.html

composer require --dev phpstan/phpstan
来源：http://hz.yueranfly.top/gtnozkwqmu.html

[U80] PHP：代码规范修复
来源：http://hz.shangyingyoupin.top/gtggpmqbej.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.chenjidiqi.icu/gtxehdoiqr.html

[U81] JS：初始化项目
来源：http://hz.fzhhl.top/gtwkbdokok.html

npm init -y;  npm i express
来源：http://hz.ydzc1.top/gtsnfbkoty.html

[U82] JS：package.json 脚本
来源：http://hz.chenjidiqi.icu/gthgobwppn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hongshengwenyu.top/gtvutxsgkf.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhengqikj.top/gtgufpmxms.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zdqjudy.top/gtggafnxxa.html

[U84] JS：CommonJS 写法
来源：http://hz.shzxlz.cn/gtmiguwfzw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jqgfzy.top/gtfyiogqsf.html

[U85] JS：可选链
来源：http://hz.gogol.net.cn/gtufitszba.html

a?.b?.c
来源：http://hz.wangshuangyany.cn/gtkphetfub.html

[U86] JS：空值合并
来源：http://hz.zycfv.cn/gtdghneuiv.html

a ?? b
来源：http://hz.redwolf501.top/gtlazicdvm.html

[U87] JS：解构默认值
来源：http://hz.snrcjt.cn/gtllqjahwv.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yonumen.top/gtmjrpecii.html

[U88] JS：对象展开合并
来源：http://hz.aibaodan.cn/gtnlhxmriq.html

{ ...a, ...b }
来源：http://hz.xylfe.cn/gtoyydyfnt.html


<!-- 参考信息 -->