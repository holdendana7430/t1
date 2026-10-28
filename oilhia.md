代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.kuanghao11.cn/gtjgcmhuft.html

[S55] C++：结构化绑定
来源：http://hz.tanke756.top/gtzvvebfow.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.kuanghao11.cn/gttodvnfbs.html

[S56] C++：optional
来源：http://hz.yj20258888.top/gtvbcghqdt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yuxming.cn/gtdkxmeyyc.html

[S57] C++：编译期常量
来源：http://hz.haohaochexian.top/gtvssicvdg.html

constexpr int N = 10;
来源：http://hz.shuidangran.top/gtdagecibg.html

[S58] C++：命名空间
来源：http://hz.mhx1999.top/gthcaiuihh.html

namespace ns { int f() { return 1; } }
来源：http://hz.shzxlz.cn/gtjhqxhycr.html

[S59] C++：静态断言
来源：http://hz.xinyue.icu/gtcoqqjzup.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jyoumei.cn/gtthqggdjb.html

[S60] C++：遍历并删除元素
来源：http://hz.gzhubu.top/gtfofufwfl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xziqi.cn/gtxecmfzcr.html

================================================================================
来源：http://hz.dianchejie.cn/gtxalsifqm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.316326.xyz/gtfudpaqpi.html

================================================================================
来源：http://hz.cucudq.cn/gtgbarpokt.html

[T01] Kotlin：Hello World
来源：http://hz.gogol.net.cn/gtihmblcmg.html

println("Hello")
来源：http://hz.yangfankeji.com/gtvvcehhdm.html

[T02] Kotlin：变量
来源：http://hz.vqdsnc.cn/gtyzgkxdkq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xuetiantiany.cn/gtfyrubqfs.html

[T03] Kotlin：字符串模板
来源：http://hz.ivvv.top/gtgbzubhug.html

"值: $b"
来源：http://hz.zhaomingkeji.xyz/gtcrjdmciy.html

[T04] Kotlin：空安全
来源：http://hz.hnqzz.top/gtsorzlsyx.html

val n: String? = null;  n?.length
来源：http://hz.hfpthk.cn/gtkqvzunqc.html

[T05] Kotlin：when 表达式
来源：http://hz.shangyingyoupin.top/gtrsdjhydc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hysaishi.cn/gthmxmghrf.html

[T06] Kotlin：集合映射
来源：http://hz.mhx1999.top/gtjwivnmno.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gogol.net.cn/gtbgokmsfu.html

[T07] Kotlin：集合过滤
来源：http://hz.hysaishi.cn/gtgkuzdmbf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xuetiantiany.cn/gthgadesgt.html

[T08] Kotlin：数据类
来源：http://hz.hnxiangtu.top/gtvstmhebx.html

data class User(val name: String, val age: Int)
来源：http://hz.yuanzhike.top/gttaxtueyk.html

[T09] Kotlin：扩展函数
来源：http://hz.smart0.xyz/gtdiwqgwnx.html

fun String.exclaim() = this + "!"
来源：http://hz.chenzaomai.com/gtnijenkod.html

[T10] Kotlin：默认参数
来源：http://hz.shanyushiyangtech.top/gtqeqzrshj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.andypj.xyz/gtnunhkfcl.html

[T11] Kotlin：协程
来源：http://hz.hfpthk.cn/gtlirspeyf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yueranfly.top/gtbtfdywut.html

[T12] Kotlin：解构声明
来源：http://hz.hongshengwenyu.top/gtkeaxoyom.html

val (a, b) = Pair(1, 2)
来源：http://hz.shangyingyoupin.top/gtqsdbewoo.html

[T13] Kotlin：只读 Map
来源：http://hz.wangdashe.top/gtewcrvvrz.html

val m = mapOf("a" to 1)
来源：http://hz.yonumen.top/gtdvkvsnbv.html

[T14] Kotlin：循环
来源：http://hz.xuetiantiany.cn/gtvlwnebdx.html

for (i in 1..10) println(i)
来源：http://hz.yangfankeji.com/gtktebqxzt.html

[T15] Kotlin：接口
来源：http://hz.quarkkingdee.top/gtpmrgrwci.html

interface Shape { fun area(): Double }
来源：http://hz.xuanzx.com/gtqngykjfw.html

[T16] Swift：Hello World
来源：http://hz.zhijiandao.cn/gttzuujeqk.html

print("Hello")
来源：http://hz.feifeiyinyue.top/gtkotdwyoy.html

[T17] Swift：变量与常量
来源：http://hz.hywenlv.cn/gtxdlpukcn.html

var a = 1;  let b = 2
来源：http://hz.zhongyouzk.top/gtgnhoirvo.html

[T18] Swift：字符串插值
来源：http://hz.xuanzx.com/gtgecqjvgs.html

"值: \(b)"
来源：http://hz.yangfankeji.com/gtcbjtgbap.html

[T19] Swift：可选绑定
来源：http://hz.zhengqikj.top/gtvnsyircd.html

if let n = opt { print(n) }
来源：http://hz.andypj.xyz/gtarpnhccn.html

[T20] Swift：数组操作
来源：http://hz.shanyushiyangkeji.top/gtyyxenvge.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xinyue.icu/gtwthrrxyn.html

[T21] Swift：遍历
来源：http://hz.vqdsnc.cn/gtmnbggcsm.html

for x in a { print(x) }
来源：http://hz.daria6918.cn/gthcbrhyry.html

[T22] Swift：字典
来源：http://hz.jinqigfzy.top/gtzjbuyjfk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhoulong.xyz/gtvebeahsg.html

[T23] Swift：函数
来源：http://hz.dashuyun.cn/gtaebtytpv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.snrcjt.cn/gtasiyjymb.html

[T24] Swift：闭包
来源：http://hz.ppjwa.cn/gtmcydugib.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.kuanghao11.cn/gtoisursgp.html

[T25] Swift：结构体
来源：http://hz.birdmap.top/gtatafysfg.html

struct P { var x: Int }
来源：http://hz.jinghuilouyu.cn/gtvbfpsbnb.html

[T26] Swift：类与重写
来源：http://hz.hammf.cn/gtmdkaidxj.html

class A: Base { override func f() {} }
来源：http://hz.ehwqpu.com/gtmqtpdzyp.html

[T27] Swift：错误处理
来源：http://hz.zhoulong.xyz/gtarxcvbbn.html

do { try f() } catch { print(error) }
来源：http://hz.dianchejie.cn/gtbedtqbds.html

[T28] Swift：枚举
来源：http://hz.jinyuanbaomall.cn/gtsiuzduec.html

enum Color { case red, green }
来源：http://hz.meibo888.top/gtvbqyjotc.html

[T29] Swift：guard 提前返回
来源：http://hz.jqgufenzy.top/gtxuyyicdn.html

guard let x = opt else { return }
来源：http://hz.mhx1999.top/gtqlgfxnai.html

[T30] Swift：协议
来源：http://hz.cheryme.top/gteuqqyzqu.html

protocol Shape { func area() -> Double }
来源：http://hz.hysaishi.cn/gtqjeezfxo.html

[T31] Lua：Hello World
来源：http://hz.andypj.xyz/gtysxtefbu.html

print("Hello")
来源：http://hz.c1oappe.top/gthsyywukr.html

[T32] Lua：局部变量
来源：http://hz.gaohongyu789.top/gtsblapapl.html

local a = 1
来源：http://hz.aizwys.cn/gtjppgxcsx.html

[T33] Lua：表（数组）
来源：http://hz.zhengqikj.top/gtvkkbzllc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.quarkkingdee.top/gtlipgbrml.html

[T34] Lua：遍历表
来源：http://hz.shzxlz.cn/gtwnygunni.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.guannengcc.top/gtetvqpydy.html

[T35] Lua：字典表
来源：http://hz.fzhhl.top/gtgxdicnse.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ehwqpu.com/gtvgfnwxnk.html

[T36] Lua：函数
来源：http://hz.jiagoushi.top/gtqixutbmo.html

function add(a, b) return a + b end
来源：http://hz.yangfankeji.com/gtpmudwfzk.html

[T37] Lua：字符串拼接
来源：http://hz.svipenyu.cn/gtngmpcarx.html

"a" .. "b"
来源：http://hz.jinyuanbaomall.cn/gtrfwwdwju.html

[T38] Lua：条件
来源：http://hz.jlsjyb.cn/gtrvkvqzax.html

if x > 0 then print("正") end
来源：http://hz.52xcode.cn/gtfvsgswoi.html

[T39] Lua：模式匹配
来源：http://hz.yangfankeji.com/gtkjfmzxgp.html

string.find(s, "%d+")
来源：http://hz.316326.xyz/gtmazcsdsk.html

[T40] Lua：元表
来源：http://hz.zhongyouzk.top/gtlvqsifrs.html

setmetatable({}, { __index = base })
来源：http://hz.zhaomingkeji.xyz/gtmoeovzue.html

[T41] Perl：Hello World
来源：http://hz.shanyushiyangkeji.top/gthyrxjysl.html

print "Hello\n";
来源：http://hz.xylfe.cn/gtdvpikstf.html

[T42] Perl：变量类型
来源：http://hz.svipenyu.cn/gtbgkujcdw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xuanzx.com/gtxfafusje.html

[T43] Perl：字符串插值
来源：http://hz.xinyue.icu/gtzntwegkh.html

"值: $a"
来源：http://hz.ivvv.top/gtzunsvtfx.html

[T44] Perl：条件
来源：http://hz.hfpthk.cn/gtasfuvlkt.html

if ($a > 0) { print "正"; }
来源：http://hz.gotoacloud.top/gtmpnnsepo.html

[T45] Perl：数组遍历
来源：http://hz.yj20258.top/gtzzmbpwvu.html

for my $x (@arr) { print $x; }
来源：http://hz.gzhubu.top/gtdsahsbxm.html

[T46] Perl：哈希操作
来源：http://hz.yanxiufei.cn/gttbnvomju.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhijiandao.cn/gtvxqzwibu.html

[T47] Perl：正则捕获
来源：http://hz.zhengqikj.top/gtenygclxr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.haohaochexian.top/gtijpamvui.html

[T48] Perl：正则替换
来源：http://hz.316326.xyz/gtbqfsdnbx.html

$s =~ s/old/new/g;
来源：http://hz.zhixingplan.top/gtigdudblq.html

[T49] Perl：函数
来源：http://hz.shanyushiyangkeji.top/gtbvogwrwv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhoulong.xyz/gtvodhwwta.html

[T50] Perl：逐行读文件
来源：http://hz.jinqigfzy.top/gtohqgbujq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gotoacloud.top/gtcokhnsao.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jqgufenzy.top/gtbdcugtjn.html

[T51] Scala：Hello World
来源：http://hz.daria6918.cn/gtnrethfpy.html

println("Hello")
来源：http://hz.cqqwz.cn/gtqzkfpyky.html

[T52] Scala：变量
来源：http://hz.yuxming.cn/gtynalbgtl.html

val a = 1;  var b = 2
来源：http://hz.svipenyu.cn/gtdagmgort.html

[T53] Scala：字符串插值
来源：http://hz.cucudq.cn/gtrwpjxend.html

s"值: $b"
来源：http://hz.316326.xyz/gtzuixmcxo.html

[T54] Scala：集合映射
来源：http://hz.jinqigufen.top/gtacuxtohh.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ppjwa.cn/gtthkscree.html

[T55] Scala：集合过滤
来源：http://hz.wangdashe.top/gtfxeymfbw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jqgfzy.top/gtpeddnxco.html

[T56] Scala：样例类
来源：http://hz.shangyingyoupin.top/gtzxozwcan.html

case class User(name: String, age: Int)
来源：http://hz.xziqi.cn/gtrfimextz.html

[T57] Scala：模式匹配
来源：http://hz.guowangkeji.top/gtbtqsvqlv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xziqi.cn/gtorpicyfe.html

[T58] Scala：函数定义
来源：http://hz.zdqjudy.top/gtzvltuqjn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shzxlz.cn/gtzovzmgbo.html

[T59] Scala：循环
来源：http://hz.yangfankeji.com/gtezrboxqt.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenlongwang.top/gtptxaogsf.html

[T60] Scala：折叠
来源：http://hz.jinqigufen.top/gtzdyoloux.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jyoumei.cn/gtzklpmfqc.html

================================================================================
来源：http://hz.yj20258.top/gtkxkuqxyn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yonumen.top/gtiwcwkkyw.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtqeebaigl.html

[U01] Py：创建虚拟环境
来源：http://hz.yuanzhike.top/gtfgkprmpn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sxryk.cn/gtxxakjzgr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yonumen.top/gthsotviyl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hnxiangtu.top/gtjznomhwi.html

[U03] Py：加载 .env 配置
来源：http://hz.gotoacloud.top/gtelhjhoew.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shuidangran.top/gtffvarcvj.html

[U04] Py：变量调试打印
来源：http://hz.shuidangran.top/gtxglyuyhw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.aibaodan.cn/gtxuaioxca.html

[U05] Py：列表去重且保序
来源：http://hz.snrcjt.cn/gtgrmhjtfs.html

list(dict.fromkeys(arr))
来源：http://hz.shuidangran.top/gtnonzlcyk.html

[U06] Py：合并两个字典
来源：http://hz.smart0.xyz/gtjvxqzvdg.html

{**a, **b}
来源：http://hz.jinyuanbaomall.cn/gtbwgburrp.html

[U07] Py：反转字典键值
来源：http://hz.zycfv.cn/gtexlqkmel.html

{v: k for k, v in d.items()}
来源：http://hz.yangfankeji.com/gtlxlfkjuc.html

[U08] Py：展平二维列表
来源：http://hz.yvedp.cn/gtgbumopwe.html

[y for x in nested for y in x]
来源：http://hz.xylfe.cn/gtcglezhqr.html

[U09] Py：字典取最大值的键
来源：http://hz.cdnleiting.top/gtodnhiesd.html

max(d, key=d.get)
来源：http://hz.zdqjudy.top/gtpzhrktqg.html

[U10] Py：按值排序字典
来源：http://hz.wangshuangyany.cn/gttxxmhfeu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jqgufenzy.top/gtosioeocu.html

[U11] Py：生成器表达式
来源：http://hz.nanxinkj.top/gtmrfhuoqg.html

(x * 2 for x in arr)
来源：http://hz.ppjwa.cn/gtzfzcizir.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hysaishi.cn/gtkkjpevxt.html

Counter(arr).most_common(3)
来源：http://hz.sysykeji.top/gtrbapxula.html

[U13] Py：固定长度队列
来源：http://hz.yvedp.cn/gtqvlypzpl.html

deque(maxlen=10)
来源：http://hz.jqgufenzy.top/gtegicabjr.html

[U14] Py：分组收集到列表
来源：http://hz.ehwqpu.com/gtwhdeqodt.html

defaultdict(list)
来源：http://hz.9152youxi.cn/gtiqejeqzu.html

[U15] Py：高精度计时
来源：http://hz.zhaomingkeji.xyz/gtmtkretss.html

t = time.perf_counter()
来源：http://hz.sxryk.cn/gtwcdlekle.html

[U16] Py：命令行参数解析
来源：http://hz.cheryme.top/gtfmxdwjqo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xuanzx.com/gtyhfnannb.html

[U17] Py：初始化日志
来源：http://hz.zycfv.cn/gtgqkfyxbc.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.guowangkeji.top/gtxzylacxb.html

[U18] Py：预编译正则
来源：http://hz.daxiang520.top/gtemhuloqv.html

pat = re.compile(r"\d+")
来源：http://hz.redwolf501.top/gtyopgymdo.html

[U19] Py：正则替换带回调
来源：http://hz.yuanzhike.top/gtmtvpdibh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yvedp.cn/gtewmzvkci.html

[U20] Py：缓存函数结果
来源：http://hz.redwolf501.top/gtyovruezo.html

@functools.lru_cache(maxsize=None)
来源：http://hz.quarkkingdee.top/gtoekvlfpq.html

[U21] Py：自定义上下文管理器
来源：http://hz.9152youxi.cn/gtcqxwnpft.html

@contextlib.contextmanager
来源：http://hz.tanke756.top/gtyimorqvj.html

[U22] Py：矩阵转置
来源：http://hz.c1oappe.top/gtikykzrmo.html

list(zip(*m))
来源：http://hz.guannengcc.top/gtcmsadoxr.html

[U23] Py：分块读取大文件
来源：http://hz.hammf.cn/gtyuivwrpt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xziqi.cn/gtaocezool.html

[U24] Py：路径操作
来源：http://hz.cheryme.top/gtnydmolsx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yj202588.top/gtelauqmjm.html

[U25] Py：CSV 按字典读
来源：http://hz.gogol.net.cn/gtdqrazugu.html

csv.DictReader(f)
来源：http://hz.kuanghao11.cn/gtsjdsqoan.html

[U26] Py：并发下载
来源：http://hz.yj20258.top/gtpxazfmsz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cucudq.cn/gtovkcwyct.html

[U27] Py：异步 HTTP
来源：http://hz.andypj.xyz/gtyvdnpaww.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xinyue.icu/gtvxvvyubh.html

[U28] Py：类型别名
来源：http://hz.aizwys.cn/gtqelozosg.html

UserId = int
来源：http://hz.mhx1999.top/gthbhrkgjp.html

[U29] Py：属性校验
来源：http://hz.yvedp.cn/gtwaddcbmy.html

@property 与 @x.setter 配合
来源：http://hz.wangshuangyany.cn/gtynthraai.html

[U30] Py：数据类
来源：http://hz.jinyuanbaomall.cn/gtvbrzudvr.html

@dataclass(slots=True)
来源：http://hz.shangyingyoupin.top/gtblztkbuj.html

[U31] Py：单测
来源：http://hz.meibo888.top/gtmznateme.html

python -m pytest -q
来源：http://hz.tanke756.top/gtlgretcvb.html

[U32] Py：代码格式化
来源：http://hz.cucudq.cn/gtkjwumqas.html

ruff format . && ruff check --fix .
来源：http://hz.jinqigufen.top/gtnfumhyaw.html

[U33] Py：打包发布
来源：http://hz.dashuyun.cn/gtkjqlrefn.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jqgufenzy.top/gtqrskcklh.html

[U34] Py：判断编码
来源：http://hz.sweek.top/gtvuhzhyrw.html

chardet.detect(raw)
来源：http://hz.zhijiandao.cn/gtbrwdpssj.html

[U35] Py：发送邮件
来源：http://hz.zhixingplan.top/gtdiwavawx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yueranfly.top/gtxksdlbro.html

[U36] Py：定时任务
来源：http://hz.shuidangran.top/gtfhktcown.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj20258888.top/gtpvumprju.html

[U37] Py：读写 Excel
来源：http://hz.havefunace.top/gtrpejdpwt.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.nwbrower.top/gtyabkoukj.html

[U38] Py：获取脚本所在目录
来源：http://hz.aibaodan.cn/gtzsuwzhfv.html

Path(__file__).resolve().parent
来源：http://hz.316326.xyz/gtvyaouqsr.html

[U39] Py：判断是否在交互环境
来源：http://hz.yj202588.top/gtyureykzu.html

sys.stdout.isatty()
来源：http://hz.zhixingplan.top/gtzuvwtwnx.html

[U40] Py：打印到标准错误
来源：http://hz.sxryk.cn/gthhsuupzp.html

print("err", file=sys.stderr)
来源：http://hz.hnxiangtu.top/gtfwvquxqy.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sufxvd.cn/gtcejdwydc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yanxiufei.cn/gtgichmezs.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.wangdashe.top/gtxfjjkzgx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.daria6918.cn/gtsaxlbfpu.html

[U43] PHP：声明命名空间
来源：http://hz.zhiwuduotai.top/gtxjykvvvt.html

namespace App\Http;
来源：http://hz.wangshuangyany.cn/gtwoccotgc.html

[U44] PHP：开启严格类型
来源：http://hz.cheryme.top/gtvfajnzgs.html

declare(strict_types=1);
来源：http://hz.sysykeji.top/gtiqvweute.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shangyingyoupin.top/gtrxnxokix.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydjk.org.cn/gtggysplii.html

[U46] PHP：可空类型
来源：http://hz.smart0.xyz/gtakvxlwsx.html

?string $name = null
来源：http://hz.pengpengdd.cyou/gtidsjjfmi.html

[U47] PHP：联合类型
来源：http://hz.meibo888.top/gttmtvpdup.html

int|string $id
来源：http://hz.zhiwuduotai.top/gtwajhtwjw.html

[U48] PHP：纯枚举
来源：http://hz.shuidangran.top/gtehwkifeu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ybcxt.top/gtxquxwwsc.html

[U49] PHP：只读属性
来源：http://hz.xylfe.cn/gtybulgalx.html

public readonly string $name
来源：http://hz.ivvv.top/gteeikvjqa.html

[U50] PHP：构造器属性提升
来源：http://hz.quarkkingdee.top/gtypacoenh.html

public function __construct(private int $id) {}
来源：http://hz.316326.xyz/gtlvpwnznu.html

[U51] PHP：数组解构
来源：http://hz.yanxiufei.cn/gtjkjrxjes.html

[$a, $b] = $arr;
来源：http://hz.daxiang520.top/gtfjehsnyo.html

[U52] PHP：箭头函数
来源：http://hz.chenlongwang.top/gtmgrauwuk.html

$double = fn($x) => $x * 2;
来源：http://hz.quarkkingdee.top/gtopsexssy.html

[U53] PHP：空合并运算符
来源：http://hz.hammf.cn/gtrsritamy.html

$v = $a ?? $b ?? "default";
来源：http://hz.sufxvd.cn/gthaxlxams.html

[U54] PHP：空安全调用
来源：http://hz.smart0.xyz/gthqeymtax.html

$obj?->method()
来源：http://hz.wangdashe.top/gtntziajkc.html

[U55] PHP：match 表达式
来源：http://hz.gaohongyu789.top/gtesazhnoy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xylfe.cn/gtyjdqaoqy.html

[U56] PHP：命名参数
来源：http://hz.ydjk.org.cn/gttugrxkil.html

f(a: 1, b: 2)
来源：http://hz.316326.xyz/gtyfwjggvo.html

[U57] PHP：字符串插值
来源：http://hz.ybcxt.top/gtuiurxfzj.html

"值: {$a}"
来源：http://hz.jinqigfzy.top/gtkjhfbgsk.html

[U58] PHP：数组三件套
来源：http://hz.52xcode.cn/gtuxmbzkgr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.0kj1m.cn/gtksnndjzq.html

[U59] PHP：自定义排序
来源：http://hz.tian-w.cn/gtfpxesuvn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigfzy.top/gtsdiiarwj.html

[U60] PHP：JSON 编解码
来源：http://hz.cheryme.top/gtwxwkedus.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.haohaochexian.top/gtmgsfgzkg.html

[U61] PHP：正则
来源：http://hz.zhiwuduotai.top/gtfthvpdhd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtgnpucddp.html

[U62] PHP：日期对象
来源：http://hz.pycfn.com/gtlvjghlmt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.quarkkingdee.top/gtehdfazeh.html

[U63] PHP：文件读写
来源：http://hz.hfpthk.cn/gtacemakty.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj20258.top/gtonbytnza.html

[U64] PHP：目录遍历
来源：http://hz.hnxiangtu.top/gthvdetrap.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zdqjudy.top/gtgxzqvmnl.html

[U65] PHP：会话
来源：http://hz.nwbrower.top/gtyipidkuw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yuanzhike.top/gtuczkeopn.html

[U66] PHP：设置 Cookie
来源：http://hz.zhengqikj.top/gtvnxbkepd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.svipenyu.cn/gtdbqhwpeu.html

[U67] PHP：处理文件上传
来源：http://hz.yvedp.cn/gttyzdjbdy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ivvv.top/gtmtjtnesw.html

[U68] PHP：PDO 连接
来源：http://hz.guowangkeji.top/gthdbqjosj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cqqwz.cn/gtjuxzgojj.html

[U69] PHP：PDO 预处理
来源：http://hz.bjfxy.top/gtqdqgvxsx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hongshengwenyu.top/gtqjlxkqti.html

[U70] PHP：PDO 事务
来源：http://hz.yueranfly.top/gtivhpbtke.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xinyue.icu/gtxfrdntfv.html

[U71] PHP：抛出异常
来源：http://hz.zhiwuduotai.top/gtfavvnlcf.html

throw new RuntimeException("失败", 500);
来源：http://hz.xziqi.cn/gtnsmotbfh.html

[U72] PHP：写错误日志
来源：http://hz.sxryk.cn/gtxojqwhto.html

error_log("失败: " . $e->getMessage());
来源：http://hz.0kj1m.cn/gtlpthmlbe.html

[U73] PHP：读取 ini 配置
来源：http://hz.jiagoushi.top/gtdrbopjyc.html

parse_ini_file("config.ini", true)
来源：http://hz.guannengcc.top/gtppunhuse.html

[U74] PHP：读取环境变量
来源：http://hz.xziqi.cn/gtbwkdgddp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.pengpengdd.cyou/gthlxtvgyj.html

[U75] PHP：依赖注入
来源：http://hz.andypj.xyz/gtelzmkurd.html

composer require psr/container
来源：http://hz.cqqwz.cn/gtiqxkxfmo.html

[U76] PHP：简单路由
来源：http://hz.zhongyouzk.top/gtdqctllcx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.aizwys.cn/gtzgysdqyb.html

[U77] PHP：模板渲染
来源：http://hz.svipenyu.cn/gttbuuhtkq.html

composer require twig/twig
来源：http://hz.yonumen.top/gtpjuxbjig.html

[U78] PHP：单元测试
来源：http://hz.daria6918.cn/gtiypkrrex.html

composer require --dev phpunit/phpunit
来源：http://hz.jinyuanbaomall.cn/gtkczmkufu.html

[U79] PHP：静态分析
来源：http://hz.dianchejie.cn/gtnremvpsb.html

composer require --dev phpstan/phpstan
来源：http://hz.jyoumei.cn/gttebgyxvm.html

[U80] PHP：代码规范修复
来源：http://hz.gotoacloud.top/gtctfiaxxs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhengqikj.top/gtymjibkmv.html


<!-- 参考信息 -->