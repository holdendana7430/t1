代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxinkj.top/gtfuxntnuy.html

[S55] C++：结构化绑定
来源：http://hz.jiagoushi.top/gtrtujwfog.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.snrcjt.cn/gttgtmgbky.html

[S56] C++：optional
来源：http://hz.zhongyouzk.top/gtglwltfjr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xuetiantiany.cn/gtbhxugmtw.html

[S57] C++：编译期常量
来源：http://hz.guowangkeji.top/gtkuhmpcoc.html

constexpr int N = 10;
来源：http://hz.cqqwz.cn/gtfseqxzmr.html

[S58] C++：命名空间
来源：http://hz.0kj1m.cn/gtuyznjytr.html

namespace ns { int f() { return 1; } }
来源：http://hz.ydzc1.top/gtmauadgnk.html

[S59] C++：静态断言
来源：http://hz.guannengcc.top/gtoediumma.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhiwuduotai.top/gtyvmatzlg.html

[S60] C++：遍历并删除元素
来源：http://hz.gogol.net.cn/gtbchmglxb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fzhhl.top/gtxirhbupw.html

================================================================================
来源：http://hz.aizwys.cn/gtgoplegyu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pycfn.com/gteiwalomt.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtfsadbmqv.html

[T01] Kotlin：Hello World
来源：http://hz.yuanzhike.top/gtvumzwbwi.html

println("Hello")
来源：http://hz.sxryk.cn/gtmbuqgjon.html

[T02] Kotlin：变量
来源：http://hz.zhoulong.xyz/gtmdvzkzml.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xuanzx.com/gtdfndsink.html

[T03] Kotlin：字符串模板
来源：http://hz.andypj.xyz/gtbrewzvag.html

"值: $b"
来源：http://hz.dianchejie.cn/gtzdahabwy.html

[T04] Kotlin：空安全
来源：http://hz.zhijiandao.cn/gtizfeapml.html

val n: String? = null;  n?.length
来源：http://hz.fzhhl.top/gtgnaenzvd.html

[T05] Kotlin：when 表达式
来源：http://hz.ydzc1.top/gtyyyaffex.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gotoacloud.top/gtxxqhxthx.html

[T06] Kotlin：集合映射
来源：http://hz.zycfv.cn/gtoexjpwan.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.havefunace.top/gtlovryobe.html

[T07] Kotlin：集合过滤
来源：http://hz.guannengcc.top/gticnwkhtd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydjk.org.cn/gthrpgwnjg.html

[T08] Kotlin：数据类
来源：http://hz.hfpthk.cn/gtexqhcfhs.html

data class User(val name: String, val age: Int)
来源：http://hz.ehwqpu.com/gtyiywpbiq.html

[T09] Kotlin：扩展函数
来源：http://hz.daxiang520.top/gtkjtmpxwu.html

fun String.exclaim() = this + "!"
来源：http://hz.jinqigufen.top/gtjasdkisr.html

[T10] Kotlin：默认参数
来源：http://hz.hongshengwenyu.top/gtokunbkrm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hfpthk.cn/gtthqiknzp.html

[T11] Kotlin：协程
来源：http://hz.ppjwa.cn/gtqkkmlnno.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hnxiangtu.top/gtrciqszba.html

[T12] Kotlin：解构声明
来源：http://hz.ybcxt.top/gtqzncrrxu.html

val (a, b) = Pair(1, 2)
来源：http://hz.redwolf501.top/gtdcawkpak.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258888.top/gtvcjcglvj.html

val m = mapOf("a" to 1)
来源：http://hz.zhoulong.xyz/gtprjjzofd.html

[T14] Kotlin：循环
来源：http://hz.chenjidiqi.icu/gtpalxrwma.html

for (i in 1..10) println(i)
来源：http://hz.gotoacloud.top/gtjxywxskk.html

[T15] Kotlin：接口
来源：http://hz.dianchejie.cn/gtjiweiqyc.html

interface Shape { fun area(): Double }
来源：http://hz.shanyushiyangkeji.top/gtglmddmsj.html

[T16] Swift：Hello World
来源：http://hz.hysaishi.cn/gtravegsfd.html

print("Hello")
来源：http://hz.hywenlv.cn/gtnokhsziu.html

[T17] Swift：变量与常量
来源：http://hz.pycfn.com/gtmlkreopm.html

var a = 1;  let b = 2
来源：http://hz.hfpthk.cn/gthblqsgka.html

[T18] Swift：字符串插值
来源：http://hz.c1oappe.top/gtaquukbwc.html

"值: \(b)"
来源：http://hz.gotoacloud.top/gtaacosxog.html

[T19] Swift：可选绑定
来源：http://hz.ydjk.org.cn/gtpityqegj.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gtubirxwgn.html

[T20] Swift：数组操作
来源：http://hz.ehwqpu.com/gtqxbkruew.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhijiandao.cn/gtwluheugz.html

[T21] Swift：遍历
来源：http://hz.zhengqikj.top/gtgodszeyc.html

for x in a { print(x) }
来源：http://hz.jlsjyb.cn/gtkwjbvbxe.html

[T22] Swift：字典
来源：http://hz.sufxvd.cn/gtezqlirgi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.dianchejie.cn/gtlzpmkxlz.html

[T23] Swift：函数
来源：http://hz.jinqigfzy.top/gtbksvseue.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.smart0.xyz/gtywavbnlo.html

[T24] Swift：闭包
来源：http://hz.ywan-chungtsiang.top/gtpbkdlqqg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jiagoushi.top/gtrytmbnrl.html

[T25] Swift：结构体
来源：http://hz.fzhhl.top/gtwjdzajzt.html

struct P { var x: Int }
来源：http://hz.cqqwz.cn/gtsrirzgoy.html

[T26] Swift：类与重写
来源：http://hz.yongpay.top/gtxxhdmesd.html

class A: Base { override func f() {} }
来源：http://hz.xingfuxueyuan.xyz/gteodyspjt.html

[T27] Swift：错误处理
来源：http://hz.xuetiantiany.cn/gtbhdbmnpc.html

do { try f() } catch { print(error) }
来源：http://hz.yongpay.top/gtfbuwrpqe.html

[T28] Swift：枚举
来源：http://hz.52xcode.cn/gtsgxflmww.html

enum Color { case red, green }
来源：http://hz.meibo888.top/gtfguehtgt.html

[T29] Swift：guard 提前返回
来源：http://hz.yvedp.cn/gtpfermmex.html

guard let x = opt else { return }
来源：http://hz.gzhubu.top/gtkzsaltdn.html

[T30] Swift：协议
来源：http://hz.yuxming.cn/gtatviijgs.html

protocol Shape { func area() -> Double }
来源：http://hz.yuxming.cn/gtonfgzuqb.html

[T31] Lua：Hello World
来源：http://hz.ehwqpu.com/gtdjqqmvfv.html

print("Hello")
来源：http://hz.cqqwz.cn/gtmhrrfuia.html

[T32] Lua：局部变量
来源：http://hz.zhixingplan.top/gthltzgpzl.html

local a = 1
来源：http://hz.yj202588.top/gtlfrwszcy.html

[T33] Lua：表（数组）
来源：http://hz.ywan-chungtsiang.top/gtyagiciss.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.0kj1m.cn/gthpqszyfc.html

[T34] Lua：遍历表
来源：http://hz.cucudq.cn/gtanuoernf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangshuangyany.cn/gtzcerkwvu.html

[T35] Lua：字典表
来源：http://hz.zycfv.cn/gtluxqmrdw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ehwqpu.com/gthqmflmlv.html

[T36] Lua：函数
来源：http://hz.zhoulong.xyz/gtdlwjhnnl.html

function add(a, b) return a + b end
来源：http://hz.hnqzz.top/gtwiimbgnr.html

[T37] Lua：字符串拼接
来源：http://hz.gzhubu.top/gtdstuoszi.html

"a" .. "b"
来源：http://hz.hywenlv.cn/gthmuagpir.html

[T38] Lua：条件
来源：http://hz.yvedp.cn/gtjtuxwzny.html

if x > 0 then print("正") end
来源：http://hz.ppjwa.cn/gtrzcbpmtg.html

[T39] Lua：模式匹配
来源：http://hz.hongshengwenyu.top/gttudkqegl.html

string.find(s, "%d+")
来源：http://hz.zycfv.cn/gtbbviosta.html

[T40] Lua：元表
来源：http://hz.zhongyouzk.top/gtridmeipq.html

setmetatable({}, { __index = base })
来源：http://hz.yangfankeji.com/gtfaribnjk.html

[T41] Perl：Hello World
来源：http://hz.gaohongyu789.top/gtmwfreztl.html

print "Hello\n";
来源：http://hz.yj20258.top/gtezrzzdja.html

[T42] Perl：变量类型
来源：http://hz.nwbrower.top/gtvavwajun.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhixingplan.top/gtxyaxuuqo.html

[T43] Perl：字符串插值
来源：http://hz.hongshengwenyu.top/gtqsidnpxi.html

"值: $a"
来源：http://hz.aizwys.cn/gtgxslxycc.html

[T44] Perl：条件
来源：http://hz.bjfxy.top/gttiirxnnh.html

if ($a > 0) { print "正"; }
来源：http://hz.hywenlv.cn/gtktbvvktp.html

[T45] Perl：数组遍历
来源：http://hz.kuanghao11.cn/gteothyunh.html

for my $x (@arr) { print $x; }
来源：http://hz.yanxiufei.cn/gtyysnbhas.html

[T46] Perl：哈希操作
来源：http://hz.gogol.net.cn/gtlinlmqvy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.aibaodan.cn/gtsbotbrze.html

[T47] Perl：正则捕获
来源：http://hz.wangdashe.top/gteyglkbil.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hammf.cn/gtzmjymwps.html

[T48] Perl：正则替换
来源：http://hz.shzxlz.cn/gtnnoevcao.html

$s =~ s/old/new/g;
来源：http://hz.pengpengdd.cyou/gtjyngfjnl.html

[T49] Perl：函数
来源：http://hz.aizwys.cn/gtecjtkgvz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cashguo.top/gtqohvllsh.html

[T50] Perl：逐行读文件
来源：http://hz.havefunace.top/gtzvfwbril.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gogol.net.cn/gtwclvbzoi.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.wangdashe.top/gtceyqapqc.html

[T51] Scala：Hello World
来源：http://hz.xuetiantiany.cn/gtisgmusut.html

println("Hello")
来源：http://hz.gogol.net.cn/gthnebrjcr.html

[T52] Scala：变量
来源：http://hz.shzxlz.cn/gtthnfivbz.html

val a = 1;  var b = 2
来源：http://hz.dianchejie.cn/gtrfmeimwn.html

[T53] Scala：字符串插值
来源：http://hz.xziqi.cn/gtlfnaqjnp.html

s"值: $b"
来源：http://hz.nanxuanxn.top/gtetowepjc.html

[T54] Scala：集合映射
来源：http://hz.zdqjudy.top/gtbvfhzyke.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hnqzz.top/gtguxmqeox.html

[T55] Scala：集合过滤
来源：http://hz.hongshengwenyu.top/gtkyischbs.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gzhubu.top/gtxluyomht.html

[T56] Scala：样例类
来源：http://hz.hammf.cn/gtvogsnfkg.html

case class User(name: String, age: Int)
来源：http://hz.zhongyouzk.top/gtrqgxrvup.html

[T57] Scala：模式匹配
来源：http://hz.yvedp.cn/gtowihfmxs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shanyushiyangtech.top/gtelcrjzeu.html

[T58] Scala：函数定义
来源：http://hz.jyoumei.cn/gtjkimyhuq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cashguo.top/gtyrhpbrjh.html

[T59] Scala：循环
来源：http://hz.fengsongda.top/gtslezxchm.html

for (i <- 1 to 10) println(i)
来源：http://hz.meibo888.top/gtiovkambv.html

[T60] Scala：折叠
来源：http://hz.ydzc1.top/gtvtmgwsqi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.birdmap.top/gtbmwezscd.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gttlufttod.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.9152youxi.cn/gtkqnmbgis.html

================================================================================
来源：http://hz.smart0.xyz/gtbmnpipkn.html

[U01] Py：创建虚拟环境
来源：http://hz.shanyushiyangkeji.top/gtrajedfny.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.nwbrower.top/gtwkqyqklj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xuanzx.com/gtmkoepntp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.aibaodan.cn/gtnvsiujml.html

[U03] Py：加载 .env 配置
来源：http://hz.daria6918.cn/gtxncowmyi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj202588.top/gtupakezrn.html

[U04] Py：变量调试打印
来源：http://hz.wangdashe.top/gtmrtdhfeb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tian-w.cn/gtdjabgakk.html

[U05] Py：列表去重且保序
来源：http://hz.dianchejie.cn/gtrvlnatlu.html

list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtzsxxlyos.html

[U06] Py：合并两个字典
来源：http://hz.yueranfly.top/gtbvqyulqv.html

{**a, **b}
来源：http://hz.smart0.xyz/gtaogcpbtg.html

[U07] Py：反转字典键值
来源：http://hz.chenlongwang.top/gttwdufwny.html

{v: k for k, v in d.items()}
来源：http://hz.yongpay.top/gtsccmbbph.html

[U08] Py：展平二维列表
来源：http://hz.pengpengdd.cyou/gttpnniupq.html

[y for x in nested for y in x]
来源：http://hz.jyoumei.cn/gtnvdkgqze.html

[U09] Py：字典取最大值的键
来源：http://hz.xuetiantiany.cn/gtqrojaikl.html

max(d, key=d.get)
来源：http://hz.jiagoushi.top/gtfdsnqusi.html

[U10] Py：按值排序字典
来源：http://hz.chenjidiqi.icu/gtuqznszto.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.tianlin.xyz/gtptodytxk.html

[U11] Py：生成器表达式
来源：http://hz.nanxuanxn.top/gtwaghwjls.html

(x * 2 for x in arr)
来源：http://hz.yvedp.cn/gtmhvgqoev.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yj20258888.top/gtvppaeyum.html

Counter(arr).most_common(3)
来源：http://hz.redwolf501.top/gtoldorsnn.html

[U13] Py：固定长度队列
来源：http://hz.sxryk.cn/gttmaektpr.html

deque(maxlen=10)
来源：http://hz.shangyingyoupin.top/gtlpiayqvx.html

[U14] Py：分组收集到列表
来源：http://hz.ppjwa.cn/gtzhrfjxhi.html

defaultdict(list)
来源：http://hz.nwbrower.top/gtnwfllafy.html

[U15] Py：高精度计时
来源：http://hz.mhx1999.top/gtilrcczfm.html

t = time.perf_counter()
来源：http://hz.dianchejie.cn/gtfzebjxwb.html

[U16] Py：命令行参数解析
来源：http://hz.svipenyu.cn/gtvgjxdxyv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.bjfxy.top/gtuertagsz.html

[U17] Py：初始化日志
来源：http://hz.sufxvd.cn/gtzargtkmf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jiagoushi.top/gtylrlndig.html

[U18] Py：预编译正则
来源：http://hz.jqgufenzy.top/gtjddftaea.html

pat = re.compile(r"\d+")
来源：http://hz.wangshuangyany.cn/gtkgxswrgf.html

[U19] Py：正则替换带回调
来源：http://hz.quarkkingdee.top/gtmzzebgky.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhixingplan.top/gteshtuuox.html

[U20] Py：缓存函数结果
来源：http://hz.zhiwuduotai.top/gtzwaoyeum.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ydzc1.top/gtasrdxbmu.html

[U21] Py：自定义上下文管理器
来源：http://hz.hysaishi.cn/gtkxnlcszl.html

@contextlib.contextmanager
来源：http://hz.zhaomingkeji.xyz/gtxhitcazk.html

[U22] Py：矩阵转置
来源：http://hz.kuanghao11.cn/gtpfoxwvxi.html

list(zip(*m))
来源：http://hz.fengsongda.top/gtsuhhksjr.html

[U23] Py：分块读取大文件
来源：http://hz.fzhhl.top/gtgkgretba.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xuanzx.com/gtweajcwai.html

[U24] Py：路径操作
来源：http://hz.jinghuilouyu.cn/gtsycaybyg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtlwxxoits.html

[U25] Py：CSV 按字典读
来源：http://hz.yangfankeji.com/gtwqecjgox.html

csv.DictReader(f)
来源：http://hz.ywan-chungtsiang.top/gtaudethop.html

[U26] Py：并发下载
来源：http://hz.redwolf501.top/gttfisfhkj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.fengsongda.top/gtflwezunm.html

[U27] Py：异步 HTTP
来源：http://hz.cqqwz.cn/gtrvdbdaqp.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.nwbrower.top/gteninzwfa.html

[U28] Py：类型别名
来源：http://hz.sufxvd.cn/gtbtpzhalf.html

UserId = int
来源：http://hz.meibo888.top/gtijznxnsl.html

[U29] Py：属性校验
来源：http://hz.yueranfly.top/gtnorjjzzz.html

@property 与 @x.setter 配合
来源：http://hz.xuetiantiany.cn/gtghtgdxym.html

[U30] Py：数据类
来源：http://hz.fzhhl.top/gtsqtxljad.html

@dataclass(slots=True)
来源：http://hz.jinyuanbaomall.cn/gtfekwpxbl.html

[U31] Py：单测
来源：http://hz.sysykeji.top/gtdvnenuyh.html

python -m pytest -q
来源：http://hz.cucudq.cn/gtfilyknta.html

[U32] Py：代码格式化
来源：http://hz.wangshuangyany.cn/gtdyyudvrb.html

ruff format . && ruff check --fix .
来源：http://hz.zhixingplan.top/gthfdkqvey.html

[U33] Py：打包发布
来源：http://hz.xziqi.cn/gtqihbkqag.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cucudq.cn/gturgbwvbu.html

[U34] Py：判断编码
来源：http://hz.ydjk.org.cn/gtucjbuykc.html

chardet.detect(raw)
来源：http://hz.ppjwa.cn/gtijnesbvo.html

[U35] Py：发送邮件
来源：http://hz.meibo888.top/gtiwnziyzq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.daria6918.cn/gtyywvbwbu.html

[U36] Py：定时任务
来源：http://hz.dianchejie.cn/gtfueydiso.html

schedule.every(10).minutes.do(job)
来源：http://hz.daxiang520.top/gtkwchmtip.html

[U37] Py：读写 Excel
来源：http://hz.hongshengwenyu.top/gtebnrizab.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhijiandao.cn/gtgizxjknp.html

[U38] Py：获取脚本所在目录
来源：http://hz.daxiang520.top/gturoypecu.html

Path(__file__).resolve().parent
来源：http://hz.quarkkingdee.top/gtbvrlcuap.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhengqikj.top/gtxfefirdx.html

sys.stdout.isatty()
来源：http://hz.hnxiangtu.top/gtwgdwrnwq.html

[U40] Py：打印到标准错误
来源：http://hz.wangdashe.top/gtrplfzenw.html

print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gtmlbuhkcm.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cdnleiting.top/gtqdbpjkqv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hfpthk.cn/gtisnlwtar.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sxryk.cn/gtqodtglfy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ywan-chungtsiang.top/gtttzyoghd.html

[U43] PHP：声明命名空间
来源：http://hz.jyoumei.cn/gtqpqsuzyl.html

namespace App\Http;
来源：http://hz.xziqi.cn/gtclmzryih.html

[U44] PHP：开启严格类型
来源：http://hz.zhaomingkeji.xyz/gtalknihsn.html

declare(strict_types=1);
来源：http://hz.zhaomingkeji.xyz/gtdklingpd.html

[U45] PHP：类型声明与返回类型
来源：http://hz.gzhubu.top/gtpjocgauh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhijiandao.cn/gtqewksczq.html

[U46] PHP：可空类型
来源：http://hz.jqgfzy.top/gtcufgtrco.html

?string $name = null
来源：http://hz.svipenyu.cn/gtitluvkce.html

[U47] PHP：联合类型
来源：http://hz.yonumen.top/gtlpmaqvtq.html

int|string $id
来源：http://hz.dianchejie.cn/gtslxjiwvu.html

[U48] PHP：纯枚举
来源：http://hz.sufxvd.cn/gtkuvqoxew.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhixingplan.top/gtdvphjztl.html

[U49] PHP：只读属性
来源：http://hz.yanxiufei.cn/gtjnsxapwz.html

public readonly string $name
来源：http://hz.gotoacloud.top/gtlejschpu.html

[U50] PHP：构造器属性提升
来源：http://hz.smart0.xyz/gtajdtnlaz.html

public function __construct(private int $id) {}
来源：http://hz.zhengqikj.top/gtpxniyzlb.html

[U51] PHP：数组解构
来源：http://hz.fengsongda.top/gtoricqoul.html

[$a, $b] = $arr;
来源：http://hz.hysaishi.cn/gtyttzgeqf.html

[U52] PHP：箭头函数
来源：http://hz.ehwqpu.com/gtztiwjcwm.html

$double = fn($x) => $x * 2;
来源：http://hz.daria6918.cn/gtpdtpokby.html

[U53] PHP：空合并运算符
来源：http://hz.snrcjt.cn/gtuuzxavga.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhaomingkeji.xyz/gtrkgeckdv.html

[U54] PHP：空安全调用
来源：http://hz.zhijiandao.cn/gtqzhbwcih.html

$obj?->method()
来源：http://hz.dianchejie.cn/gtjrshcujs.html

[U55] PHP：match 表达式
来源：http://hz.zhixingplan.top/gtjffoutlk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.andypj.xyz/gtxdiboztj.html

[U56] PHP：命名参数
来源：http://hz.tianlin.xyz/gtukvwfbrd.html

f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtnekezcjq.html

[U57] PHP：字符串插值
来源：http://hz.gotoacloud.top/gtlznuyybz.html

"值: {$a}"
来源：http://hz.sysykeji.top/gtcrtrbrrj.html

[U58] PHP：数组三件套
来源：http://hz.zhiwuduotai.top/gtfiasvrwt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.guowangkeji.top/gtozzropbe.html

[U59] PHP：自定义排序
来源：http://hz.xingfuxueyuan.xyz/gtgccizhcu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hammf.cn/gtrhfkebqm.html

[U60] PHP：JSON 编解码
来源：http://hz.hnxiangtu.top/gthwdfmwfu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.sysykeji.top/gtnwqktxnd.html

[U61] PHP：正则
来源：http://hz.ywan-chungtsiang.top/gtiousqfep.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuanzx.com/gtsmgggwjm.html

[U62] PHP：日期对象
来源：http://hz.0kj1m.cn/gtburtmmuy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yvedp.cn/gtpewotycc.html

[U63] PHP：文件读写
来源：http://hz.hysaishi.cn/gtemlmmrdq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.birdmap.top/gtjzxunpxy.html

[U64] PHP：目录遍历
来源：http://hz.sysykeji.top/gtdtsfbjxl.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sweek.top/gtlpwexlkq.html

[U65] PHP：会话
来源：http://hz.wangdashe.top/gtvewuqeeh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hnqzz.top/gtharhstrs.html

[U66] PHP：设置 Cookie
来源：http://hz.nwbrower.top/gtdkcrwben.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jqgfzy.top/gtirhaskaw.html

[U67] PHP：处理文件上传
来源：http://hz.zhoulong.xyz/gtxourigez.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jinqigufen.top/gtbfyauhqg.html

[U68] PHP：PDO 连接
来源：http://hz.zdqjudy.top/gtggzataqz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shanyushiyangtech.top/gtajdgyzrd.html

[U69] PHP：PDO 预处理
来源：http://hz.ehwqpu.com/gtjtcanccr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ppjwa.cn/gtzrqewrgo.html

[U70] PHP：PDO 事务
来源：http://hz.yueranfly.top/gtedfliuty.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.iojbl.cn/gtbtstlgid.html

[U71] PHP：抛出异常
来源：http://hz.sxryk.cn/gtmvppcgrc.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhaomingkeji.xyz/gtwtvgrjld.html

[U72] PHP：写错误日志
来源：http://hz.shuidangran.top/gtpufobngp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.xylfe.cn/gtpnhihzya.html

[U73] PHP：读取 ini 配置
来源：http://hz.xinyue.icu/gthodxsojj.html

parse_ini_file("config.ini", true)
来源：http://hz.mhx1999.top/gtmoxhsfhx.html

[U74] PHP：读取环境变量
来源：http://hz.gogol.net.cn/gtglctbdoa.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yanxiufei.cn/gtgzjylujm.html

[U75] PHP：依赖注入
来源：http://hz.hammf.cn/gtijoliwet.html

composer require psr/container
来源：http://hz.sysykeji.top/gtjfbsmwct.html

[U76] PHP：简单路由
来源：http://hz.xingfuxueyuan.xyz/gtwvemonmf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhiwuduotai.top/gtpknggpol.html

[U77] PHP：模板渲染
来源：http://hz.sysykeji.top/gtybevgqgy.html

composer require twig/twig
来源：http://hz.zhengqikj.top/gtnwhbxqdq.html

[U78] PHP：单元测试
来源：http://hz.wangshuangyany.cn/gthxqzrztn.html

composer require --dev phpunit/phpunit
来源：http://hz.jinqigfzy.top/gtngnrwogi.html

[U79] PHP：静态分析
来源：http://hz.nanxuanxn.top/gtqklziacp.html

composer require --dev phpstan/phpstan
来源：http://hz.shzxlz.cn/gtwfvoolgx.html

[U80] PHP：代码规范修复
来源：http://hz.ydzc1.top/gtvuaiwidu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.0kj1m.cn/gtplymosob.html


<!-- 参考信息 -->