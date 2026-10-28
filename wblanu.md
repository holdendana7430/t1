代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhengqikj.top/gtpjiejvpt.html

[S55] C++：结构化绑定
来源：http://hz.yvedp.cn/gtmdbgklmz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.redwolf501.top/gtoicttjnd.html

[S56] C++：optional
来源：http://hz.pengpengdd.cyou/gtyqvlvxky.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cucudq.cn/gtvdniipbq.html

[S57] C++：编译期常量
来源：http://hz.ybcxt.top/gtvyfcowym.html

constexpr int N = 10;
来源：http://hz.hongshengwenyu.top/gthwqbacxb.html

[S58] C++：命名空间
来源：http://hz.jiagoushi.top/gtoyvgaqlv.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj202588.top/gtomxoirfl.html

[S59] C++：静态断言
来源：http://hz.cucudq.cn/gtzhnnpaaw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhoulong.xyz/gtvyulolkv.html

[S60] C++：遍历并删除元素
来源：http://hz.tanke756.top/gtstlwgmuc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fengsongda.top/gtbpbgnoby.html

================================================================================
来源：http://hz.hysaishi.cn/gtxrmpzfzk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigufen.top/gtcovotdpk.html

================================================================================
来源：http://hz.iojbl.cn/gtzesfutyj.html

[T01] Kotlin：Hello World
来源：http://hz.chenjidiqi.icu/gtzhrovtqx.html

println("Hello")
来源：http://hz.zhongyouzk.top/gtuczlhera.html

[T02] Kotlin：变量
来源：http://hz.zhijiandao.cn/gtjbjbcsvj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jyoumei.cn/gtgekqojiy.html

[T03] Kotlin：字符串模板
来源：http://hz.zhongyouzk.top/gtysyeotzf.html

"值: $b"
来源：http://hz.zhengqikj.top/gtjdblgkzx.html

[T04] Kotlin：空安全
来源：http://hz.cashguo.top/gtnqgcyirz.html

val n: String? = null;  n?.length
来源：http://hz.ydjk.org.cn/gtoywlybon.html

[T05] Kotlin：when 表达式
来源：http://hz.iojbl.cn/gtoipwlbeo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shzxlz.cn/gttmkoftwe.html

[T06] Kotlin：集合映射
来源：http://hz.nwbrower.top/gtgwxwrpqn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hammf.cn/gtqbvgpvun.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258.top/gtprozzdqh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.birdmap.top/gtmdudbyqj.html

[T08] Kotlin：数据类
来源：http://hz.hammf.cn/gtnmowlawe.html

data class User(val name: String, val age: Int)
来源：http://hz.sufxvd.cn/gtxgrxpusz.html

[T09] Kotlin：扩展函数
来源：http://hz.9152youxi.cn/gtqqkuagio.html

fun String.exclaim() = this + "!"
来源：http://hz.yuxming.cn/gtugwcmysw.html

[T10] Kotlin：默认参数
来源：http://hz.jinyuanbaomall.cn/gtkanfghxx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jianghu66.top/gtstmiuhey.html

[T11] Kotlin：协程
来源：http://hz.52xcode.cn/gtknzxtewn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sxryk.cn/gtsdbfrxxz.html

[T12] Kotlin：解构声明
来源：http://hz.cqqwz.cn/gttkuncdrk.html

val (a, b) = Pair(1, 2)
来源：http://hz.cheryme.top/gtwnebfacb.html

[T13] Kotlin：只读 Map
来源：http://hz.jiagoushi.top/gtntzitesv.html

val m = mapOf("a" to 1)
来源：http://hz.mhx1999.top/gtweyyqhdq.html

[T14] Kotlin：循环
来源：http://hz.sweek.top/gtywpmoujj.html

for (i in 1..10) println(i)
来源：http://hz.c1oappe.top/gtowqrkbqy.html

[T15] Kotlin：接口
来源：http://hz.cucudq.cn/gtyoglkrmt.html

interface Shape { fun area(): Double }
来源：http://hz.guowangkeji.top/gtxwmkdugp.html

[T16] Swift：Hello World
来源：http://hz.zhoulong.xyz/gtyhkmycrb.html

print("Hello")
来源：http://hz.zhijiandao.cn/gtqmbbvyyf.html

[T17] Swift：变量与常量
来源：http://hz.shuidangran.top/gtxzttietc.html

var a = 1;  let b = 2
来源：http://hz.zycfv.cn/gtjhlciise.html

[T18] Swift：字符串插值
来源：http://hz.zhongyouzk.top/gtxlltwnxf.html

"值: \(b)"
来源：http://hz.aibaodan.cn/gtveegooxd.html

[T19] Swift：可选绑定
来源：http://hz.birdmap.top/gtqmzihczd.html

if let n = opt { print(n) }
来源：http://hz.redwolf501.top/gtkwuwazds.html

[T20] Swift：数组操作
来源：http://hz.jqgfzy.top/gtjauogenc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jqgfzy.top/gtxbcixwbs.html

[T21] Swift：遍历
来源：http://hz.feifeiyinyue.top/gtfiucilja.html

for x in a { print(x) }
来源：http://hz.ybcxt.top/gtqaihqqks.html

[T22] Swift：字典
来源：http://hz.aibaodan.cn/gtaaloavdc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sweek.top/gtqhsghfdl.html

[T23] Swift：函数
来源：http://hz.wangdashe.top/gtourkrgna.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.birdmap.top/gtvkdblsix.html

[T24] Swift：闭包
来源：http://hz.0kj1m.cn/gtcbvsllqm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yanxiufei.cn/gtvxkgpfwp.html

[T25] Swift：结构体
来源：http://hz.zhaomingkeji.xyz/gtztcnlzfw.html

struct P { var x: Int }
来源：http://hz.jinqigfzy.top/gtyhhjbztg.html

[T26] Swift：类与重写
来源：http://hz.redwolf501.top/gtfmasurln.html

class A: Base { override func f() {} }
来源：http://hz.xziqi.cn/gtbswaofnm.html

[T27] Swift：错误处理
来源：http://hz.shangyingyoupin.top/gtnnllvhyk.html

do { try f() } catch { print(error) }
来源：http://hz.zhiwuduotai.top/gtigselrom.html

[T28] Swift：枚举
来源：http://hz.jyoumei.cn/gtxzimgfpp.html

enum Color { case red, green }
来源：http://hz.pycfn.com/gtdkzbcapf.html

[T29] Swift：guard 提前返回
来源：http://hz.pengpengdd.cyou/gtcyofllyc.html

guard let x = opt else { return }
来源：http://hz.guowangkeji.top/gtkhiwmxma.html

[T30] Swift：协议
来源：http://hz.zhengqikj.top/gtkjwsbalr.html

protocol Shape { func area() -> Double }
来源：http://hz.9152youxi.cn/gtjgbcnnxk.html

[T31] Lua：Hello World
来源：http://hz.daria6918.cn/gthqeafbod.html

print("Hello")
来源：http://hz.guowangkeji.top/gtrlssnquc.html

[T32] Lua：局部变量
来源：http://hz.aibaodan.cn/gtfvhoiugm.html

local a = 1
来源：http://hz.cucudq.cn/gtkcmdlzgk.html

[T33] Lua：表（数组）
来源：http://hz.yuxming.cn/gttyirarkf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shanyushiyangtech.top/gtilpjwbsu.html

[T34] Lua：遍历表
来源：http://hz.aizwys.cn/gtlevvxhrx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinyuanbaomall.cn/gtltuxwhaf.html

[T35] Lua：字典表
来源：http://hz.yangfankeji.com/gtvafcceti.html

local d = { a = 1 };  d.b = 2
来源：http://hz.guowangkeji.top/gtdywdugjm.html

[T36] Lua：函数
来源：http://hz.zhongyouzk.top/gtmcjbcngr.html

function add(a, b) return a + b end
来源：http://hz.aibaodan.cn/gtdszjvnai.html

[T37] Lua：字符串拼接
来源：http://hz.vqdsnc.cn/gtklrsazjj.html

"a" .. "b"
来源：http://hz.9152youxi.cn/gtoxajzcmo.html

[T38] Lua：条件
来源：http://hz.sweek.top/gtfpuhxeks.html

if x > 0 then print("正") end
来源：http://hz.quarkkingdee.top/gtbeobpwwg.html

[T39] Lua：模式匹配
来源：http://hz.cqqwz.cn/gteufekmog.html

string.find(s, "%d+")
来源：http://hz.zhixingplan.top/gtunucljxf.html

[T40] Lua：元表
来源：http://hz.dashuyun.cn/gtsnofbvka.html

setmetatable({}, { __index = base })
来源：http://hz.yonumen.top/gtrbgjmuig.html

[T41] Perl：Hello World
来源：http://hz.ppjwa.cn/gteytjbmrh.html

print "Hello\n";
来源：http://hz.fengsongda.top/gtzetroonl.html

[T42] Perl：变量类型
来源：http://hz.guannengcc.top/gtnzaqexpf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj202588.top/gtkhmssdna.html

[T43] Perl：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtqwhrizmz.html

"值: $a"
来源：http://hz.0kj1m.cn/gtmiowxyzn.html

[T44] Perl：条件
来源：http://hz.dianchejie.cn/gtrezzoxfg.html

if ($a > 0) { print "正"; }
来源：http://hz.snrcjt.cn/gtsuusdslo.html

[T45] Perl：数组遍历
来源：http://hz.sysykeji.top/gttatrklhq.html

for my $x (@arr) { print $x; }
来源：http://hz.yvedp.cn/gtczuarzzt.html

[T46] Perl：哈希操作
来源：http://hz.yuxming.cn/gteunlwaiz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.meibo888.top/gtmtzxqijp.html

[T47] Perl：正则捕获
来源：http://hz.ydzc1.top/gtjgeqxdms.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zdqjudy.top/gtaecdaksa.html

[T48] Perl：正则替换
来源：http://hz.pycfn.com/gtwalyajgb.html

$s =~ s/old/new/g;
来源：http://hz.haohaochexian.top/gtoxebzflc.html

[T49] Perl：函数
来源：http://hz.yuxming.cn/gtbkkslhkk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtrktukpjq.html

[T50] Perl：逐行读文件
来源：http://hz.xuanzx.com/gtpduocxjn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xinyue.icu/gtxpeuaizd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shanyushiyangtech.top/gtyorfkbvi.html

[T51] Scala：Hello World
来源：http://hz.andypj.xyz/gthsipcosk.html

println("Hello")
来源：http://hz.yongpay.top/gtahtfuaiz.html

[T52] Scala：变量
来源：http://hz.zhaomingkeji.xyz/gtuddlixhe.html

val a = 1;  var b = 2
来源：http://hz.gotoacloud.top/gtfuvlxzwc.html

[T53] Scala：字符串插值
来源：http://hz.cdnleiting.top/gtbgtogtkd.html

s"值: $b"
来源：http://hz.shanyushiyangkeji.top/gtekeglndx.html

[T54] Scala：集合映射
来源：http://hz.jlsjyb.cn/gtndxovble.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.0kj1m.cn/gtkcajnptc.html

[T55] Scala：集合过滤
来源：http://hz.wangdashe.top/gthqqpcpss.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhixingplan.top/gtwdomrivn.html

[T56] Scala：样例类
来源：http://hz.jqgfzy.top/gtzoxukxjj.html

case class User(name: String, age: Int)
来源：http://hz.jiagoushi.top/gteaojcxps.html

[T57] Scala：模式匹配
来源：http://hz.jinqigufen.top/gtowpndfrq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cheryme.top/gtmsrwgjxe.html

[T58] Scala：函数定义
来源：http://hz.zhoulong.xyz/gtnqvtjhgd.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sufxvd.cn/gtjspskkhn.html

[T59] Scala：循环
来源：http://hz.zhiwuduotai.top/gtiskzyjms.html

for (i <- 1 to 10) println(i)
来源：http://hz.birdmap.top/gtbiaxbhmn.html

[T60] Scala：折叠
来源：http://hz.gaohongyu789.top/gtdbaijrhs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.kuanghao11.cn/gtzqbfapwr.html

================================================================================
来源：http://hz.zhongyouzk.top/gtokueghus.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xziqi.cn/gtnsvhiyuo.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtttjzmlsw.html

[U01] Py：创建虚拟环境
来源：http://hz.sxryk.cn/gtcgbijfyz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj202588.top/gtlabjpbjf.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hysaishi.cn/gtocgqjmib.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenjidiqi.icu/gtxzwnkuao.html

[U03] Py：加载 .env 配置
来源：http://hz.yangfankeji.com/gthjeoovcy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tanke756.top/gtemglqqqo.html

[U04] Py：变量调试打印
来源：http://hz.zhoulong.xyz/gtcfzoxfqt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ppjwa.cn/gtdomynzee.html

[U05] Py：列表去重且保序
来源：http://hz.ydzc1.top/gtvcpdwfzz.html

list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gtrvvdzftb.html

[U06] Py：合并两个字典
来源：http://hz.hammf.cn/gtpwpvdknk.html

{**a, **b}
来源：http://hz.guowangkeji.top/gtwgmateob.html

[U07] Py：反转字典键值
来源：http://hz.shanyushiyangkeji.top/gtbwzjufht.html

{v: k for k, v in d.items()}
来源：http://hz.jlsjyb.cn/gtapqsyfhp.html

[U08] Py：展平二维列表
来源：http://hz.zhengqikj.top/gtdtrgnvvd.html

[y for x in nested for y in x]
来源：http://hz.yj20258888.top/gtwtpxhowf.html

[U09] Py：字典取最大值的键
来源：http://hz.shangyingyoupin.top/gtkazkgurf.html

max(d, key=d.get)
来源：http://hz.cucudq.cn/gtqfypgjoa.html

[U10] Py：按值排序字典
来源：http://hz.yj20258.top/gtpwcwnjtd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhijiandao.cn/gtjdundkif.html

[U11] Py：生成器表达式
来源：http://hz.52xcode.cn/gtcgejfwzj.html

(x * 2 for x in arr)
来源：http://hz.cashguo.top/gtkliazwlg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.9152youxi.cn/gttdikktfk.html

Counter(arr).most_common(3)
来源：http://hz.yvedp.cn/gtshkywnth.html

[U13] Py：固定长度队列
来源：http://hz.meibo888.top/gttyjxykhd.html

deque(maxlen=10)
来源：http://hz.cqqwz.cn/gtofmcsibh.html

[U14] Py：分组收集到列表
来源：http://hz.yj20258.top/gtjzsjylsy.html

defaultdict(list)
来源：http://hz.tian-w.cn/gtyzizpcnp.html

[U15] Py：高精度计时
来源：http://hz.quarkkingdee.top/gtgiwoknmw.html

t = time.perf_counter()
来源：http://hz.hnxiangtu.top/gtgjhhejde.html

[U16] Py：命令行参数解析
来源：http://hz.316326.xyz/gtcbvbxydo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.shzxlz.cn/gtlnbwaesg.html

[U17] Py：初始化日志
来源：http://hz.jqgufenzy.top/gtcvjsvyls.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhengqikj.top/gtlmwonnpk.html

[U18] Py：预编译正则
来源：http://hz.fengsongda.top/gtfvkblvnr.html

pat = re.compile(r"\d+")
来源：http://hz.gotoacloud.top/gtcbozynor.html

[U19] Py：正则替换带回调
来源：http://hz.316326.xyz/gtlfbxtrhp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.meibo888.top/gtiwoflnbp.html

[U20] Py：缓存函数结果
来源：http://hz.xziqi.cn/gtsasipshn.html

@functools.lru_cache(maxsize=None)
来源：http://hz.tianlin.xyz/gtuolfwbmi.html

[U21] Py：自定义上下文管理器
来源：http://hz.gotoacloud.top/gtnswkvcnz.html

@contextlib.contextmanager
来源：http://hz.shanyushiyangkeji.top/gtdlhhwhan.html

[U22] Py：矩阵转置
来源：http://hz.nanxinkj.top/gtgminazzy.html

list(zip(*m))
来源：http://hz.birdmap.top/gtvnwvmspt.html

[U23] Py：分块读取大文件
来源：http://hz.chenjidiqi.icu/gtczhcwipr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yonumen.top/gtjtcbhvyr.html

[U24] Py：路径操作
来源：http://hz.chenlongwang.top/gtytnxliff.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.c1oappe.top/gtyxwthtyo.html

[U25] Py：CSV 按字典读
来源：http://hz.andypj.xyz/gtgsqtchhd.html

csv.DictReader(f)
来源：http://hz.kuanghao11.cn/gtwnezjrfd.html

[U26] Py：并发下载
来源：http://hz.fzhhl.top/gtrgpmxdhe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.9152youxi.cn/gtccdhrymy.html

[U27] Py：异步 HTTP
来源：http://hz.shuidangran.top/gttulhmwer.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yueranfly.top/gtucqcolri.html

[U28] Py：类型别名
来源：http://hz.nanxinkj.top/gtfeelqten.html

UserId = int
来源：http://hz.shzxlz.cn/gtrxgdgrwt.html

[U29] Py：属性校验
来源：http://hz.daria6918.cn/gtgzokcenj.html

@property 与 @x.setter 配合
来源：http://hz.hnqzz.top/gtyrmsflui.html

[U30] Py：数据类
来源：http://hz.ehwqpu.com/gttniwpjtu.html

@dataclass(slots=True)
来源：http://hz.ppjwa.cn/gtctawiwqd.html

[U31] Py：单测
来源：http://hz.haohaochexian.top/gtaslffzve.html

python -m pytest -q
来源：http://hz.sxryk.cn/gtnsgkvklr.html

[U32] Py：代码格式化
来源：http://hz.feifeiyinyue.top/gttiytaywe.html

ruff format . && ruff check --fix .
来源：http://hz.dianchejie.cn/gtgmqlwlct.html

[U33] Py：打包发布
来源：http://hz.yonumen.top/gthviybohv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.52xcode.cn/gtnfbbkgeu.html

[U34] Py：判断编码
来源：http://hz.ehwqpu.com/gttdxyosxa.html

chardet.detect(raw)
来源：http://hz.xylfe.cn/gtqhkmwbef.html

[U35] Py：发送邮件
来源：http://hz.jinyuanbaomall.cn/gtgewrrnis.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.dashuyun.cn/gtmvncttzk.html

[U36] Py：定时任务
来源：http://hz.chenjidiqi.icu/gtwztzjnvz.html

schedule.every(10).minutes.do(job)
来源：http://hz.gogol.net.cn/gtlapkxoer.html

[U37] Py：读写 Excel
来源：http://hz.yonumen.top/gtummiywll.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xziqi.cn/gtfkqsslib.html

[U38] Py：获取脚本所在目录
来源：http://hz.jyoumei.cn/gtghmreexw.html

Path(__file__).resolve().parent
来源：http://hz.guannengcc.top/gtenwqlukr.html

[U39] Py：判断是否在交互环境
来源：http://hz.jlsjyb.cn/gtbsxewlih.html

sys.stdout.isatty()
来源：http://hz.yuanzhike.top/gtfaqymjew.html

[U40] Py：打印到标准错误
来源：http://hz.chenjidiqi.icu/gtyzqznplx.html

print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtiaufypts.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.aibaodan.cn/gteyqftxqe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.dianchejie.cn/gtfkacmbep.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yuxming.cn/gtvbizkqmb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ydjk.org.cn/gtlvtprwbt.html

[U43] PHP：声明命名空间
来源：http://hz.xinyue.icu/gtsvrswqkz.html

namespace App\Http;
来源：http://hz.zhixingplan.top/gtmttilvsg.html

[U44] PHP：开启严格类型
来源：http://hz.jiagoushi.top/gtdjbwexcy.html

declare(strict_types=1);
来源：http://hz.nanxinkj.top/gtvlfxojbv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.nwbrower.top/gtmsujpuyk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gtfnsznasg.html

[U46] PHP：可空类型
来源：http://hz.9152youxi.cn/gtagugpaqd.html

?string $name = null
来源：http://hz.haohaochexian.top/gtctbclcvc.html

[U47] PHP：联合类型
来源：http://hz.feifeiyinyue.top/gtqoadxitd.html

int|string $id
来源：http://hz.hammf.cn/gthpqtldsi.html

[U48] PHP：纯枚举
来源：http://hz.wangshuangyany.cn/gtwgmqhfmj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.c1oappe.top/gtnazkbbtb.html

[U49] PHP：只读属性
来源：http://hz.pycfn.com/gtgwrupahp.html

public readonly string $name
来源：http://hz.daxiang520.top/gtybbfcfxs.html

[U50] PHP：构造器属性提升
来源：http://hz.yueranfly.top/gtzzpghzhf.html

public function __construct(private int $id) {}
来源：http://hz.fengsongda.top/gttaruccyd.html

[U51] PHP：数组解构
来源：http://hz.aibaodan.cn/gtwwvueabh.html

[$a, $b] = $arr;
来源：http://hz.xuanzx.com/gtznnpqpza.html

[U52] PHP：箭头函数
来源：http://hz.jlsjyb.cn/gtpvomwlsi.html

$double = fn($x) => $x * 2;
来源：http://hz.fengsongda.top/gtvwcyqxxt.html

[U53] PHP：空合并运算符
来源：http://hz.vqdsnc.cn/gthbwfwilj.html

$v = $a ?? $b ?? "default";
来源：http://hz.ydjk.org.cn/gtjruqmfkm.html

[U54] PHP：空安全调用
来源：http://hz.hnqzz.top/gtivhsnlcw.html

$obj?->method()
来源：http://hz.kuanghao11.cn/gtcoraruzv.html

[U55] PHP：match 表达式
来源：http://hz.svipenyu.cn/gtfmpenggw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.svipenyu.cn/gtnsjnihle.html

[U56] PHP：命名参数
来源：http://hz.aibaodan.cn/gtlwioywbp.html

f(a: 1, b: 2)
来源：http://hz.chenzaomai.com/gtcnacsgvi.html

[U57] PHP：字符串插值
来源：http://hz.jinqigufen.top/gtiysqgxff.html

"值: {$a}"
来源：http://hz.sxryk.cn/gtxrbjvvcs.html

[U58] PHP：数组三件套
来源：http://hz.yvedp.cn/gtbdjhisnb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hnxiangtu.top/gtgpqrbxhi.html

[U59] PHP：自定义排序
来源：http://hz.daria6918.cn/gtfzoxhxgb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hfpthk.cn/gtmphprlgo.html

[U60] PHP：JSON 编解码
来源：http://hz.vqdsnc.cn/gtafaqxpyb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.tian-w.cn/gteybdzhia.html

[U61] PHP：正则
来源：http://hz.yonumen.top/gtrjocxpyl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gtnhvwsxdq.html

[U62] PHP：日期对象
来源：http://hz.hongshengwenyu.top/gtdyjjmofu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.tian-w.cn/gtiirqzxlq.html

[U63] PHP：文件读写
来源：http://hz.nwbrower.top/gtqhxlwtqh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinqigfzy.top/gtmbyozjhc.html

[U64] PHP：目录遍历
来源：http://hz.jinyuanbaomall.cn/gtaxrktjjt.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.52xcode.cn/gttlhoaqua.html

[U65] PHP：会话
来源：http://hz.xinyue.icu/gtcircpclw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.tianlin.xyz/gttkmjeljc.html

[U66] PHP：设置 Cookie
来源：http://hz.daxiang520.top/gtslxmbtsl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xziqi.cn/gthlofzuqs.html

[U67] PHP：处理文件上传
来源：http://hz.gaohongyu789.top/gtermubeua.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.chenlongwang.top/gtdhosjybg.html

[U68] PHP：PDO 连接
来源：http://hz.shuidangran.top/gtowwndvnn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.52xcode.cn/gtrqtxbkjg.html

[U69] PHP：PDO 预处理
来源：http://hz.yj20258.top/gtbwfdqhlt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hongshengwenyu.top/gtcjjwpxuj.html

[U70] PHP：PDO 事务
来源：http://hz.svipenyu.cn/gtoolgfnsg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.gogol.net.cn/gtnwcqskww.html

[U71] PHP：抛出异常
来源：http://hz.xingfuxueyuan.xyz/gtolvhkroy.html

throw new RuntimeException("失败", 500);
来源：http://hz.aizwys.cn/gtnmnijihj.html

[U72] PHP：写错误日志
来源：http://hz.shanyushiyangkeji.top/gtmrbfxabv.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ydzc1.top/gtdbjjaekn.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhengqikj.top/gtsmceubei.html

parse_ini_file("config.ini", true)
来源：http://hz.havefunace.top/gtbcndawtp.html

[U74] PHP：读取环境变量
来源：http://hz.cqqwz.cn/gtcckdioxi.html

getenv("APP_ENV") ?: "production"
来源：http://hz.nanxinkj.top/gtojeeijbw.html

[U75] PHP：依赖注入
来源：http://hz.quarkkingdee.top/gtewpbfjti.html

composer require psr/container
来源：http://hz.sysykeji.top/gtcpzkwpcg.html

[U76] PHP：简单路由
来源：http://hz.shanyushiyangtech.top/gtewzazpcq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.c1oappe.top/gtsaczpztw.html

[U77] PHP：模板渲染
来源：http://hz.ivvv.top/gtsparugek.html

composer require twig/twig
来源：http://hz.sweek.top/gtmoyxskkp.html

[U78] PHP：单元测试
来源：http://hz.aizwys.cn/gtnnziboif.html

composer require --dev phpunit/phpunit
来源：http://hz.yuanzhike.top/gtxsrhbhjq.html

[U79] PHP：静态分析
来源：http://hz.jlsjyb.cn/gthtucnczb.html

composer require --dev phpstan/phpstan
来源：http://hz.dashuyun.cn/gtgxnatwlk.html

[U80] PHP：代码规范修复
来源：http://hz.yj20258.top/gtsfxovmxp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.redwolf501.top/gtyegfgiex.html


<!-- 参考信息 -->