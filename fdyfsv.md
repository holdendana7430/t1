代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hywenlv.cn/gtjihmzkts.html

[S51] C++：显式类型转换
来源：http://hz.9152youxi.cn/gthxhrgzch.html

static_cast<double>(a) / b
来源：http://hz.sxryk.cn/gtgyigknnr.html

[S52] C++：const 与 noexcept
来源：http://hz.yj202588.top/gtumnfgnrg.html

int size() const noexcept { return n_; }
来源：http://hz.52xcode.cn/gthhfvggkw.html

[S53] C++：移动语义
来源：http://hz.bjfxy.top/gtegkvbjva.html

std::vector<int> w = std::move(v);
来源：http://hz.tanke756.top/gtgimvwpaj.html

[S54] C++：异常处理
来源：http://hz.wangdashe.top/gttqldxopx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cqqwz.cn/gtzovmyoqk.html

[S55] C++：结构化绑定
来源：http://hz.snrcjt.cn/gtrzqjhcdj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.guannengcc.top/gtziwcnaqq.html

[S56] C++：optional
来源：http://hz.jinghuilouyu.cn/gthamvgyjj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dashuyun.cn/gtrpokvgnb.html

[S57] C++：编译期常量
来源：http://hz.iojbl.cn/gtkqiinhxx.html

constexpr int N = 10;
来源：http://hz.sysykeji.top/gtvtwenpve.html

[S58] C++：命名空间
来源：http://hz.jinghuilouyu.cn/gtygbknyyt.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhiwuduotai.top/gtzrajpsth.html

[S59] C++：静态断言
来源：http://hz.zhengqikj.top/gtthrcijdq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gaohongyu789.top/gtfguwjysj.html

[S60] C++：遍历并删除元素
来源：http://hz.tianlin.xyz/gtnlyttsfd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.vqdsnc.cn/gtwczbhdnu.html

================================================================================
来源：http://hz.aibaodan.cn/gtcairnxtb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tianlin.xyz/gtmpfxklrt.html

================================================================================
来源：http://hz.hfpthk.cn/gtxbndehac.html

[T01] Kotlin：Hello World
来源：http://hz.nanxuanxn.top/gttlclldpi.html

println("Hello")
来源：http://hz.nwbrower.top/gtmpndvhyr.html

[T02] Kotlin：变量
来源：http://hz.jianghu66.top/gtyubewild.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yongpay.top/gtkqiggmec.html

[T03] Kotlin：字符串模板
来源：http://hz.dianchejie.cn/gtbvwnqhbs.html

"值: $b"
来源：http://hz.jinyuanbaomall.cn/gtraqwvwfx.html

[T04] Kotlin：空安全
来源：http://hz.svipenyu.cn/gtrmoqthzz.html

val n: String? = null;  n?.length
来源：http://hz.jyoumei.cn/gtncryxqfd.html

[T05] Kotlin：when 表达式
来源：http://hz.jlsjyb.cn/gtlgixzxfa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yvedp.cn/gtrrtacmde.html

[T06] Kotlin：集合映射
来源：http://hz.tianlin.xyz/gtwtjqsgbn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.havefunace.top/gtmnrzuuav.html

[T07] Kotlin：集合过滤
来源：http://hz.zhiwuduotai.top/gtrrcssxhq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pengpengdd.cyou/gtbkiedvmz.html

[T08] Kotlin：数据类
来源：http://hz.nanxuanxn.top/gtpylobeke.html

data class User(val name: String, val age: Int)
来源：http://hz.sysykeji.top/gthhlmitvy.html

[T09] Kotlin：扩展函数
来源：http://hz.mhx1999.top/gtymjdhbrq.html

fun String.exclaim() = this + "!"
来源：http://hz.zhixingplan.top/gtdmcfspbh.html

[T10] Kotlin：默认参数
来源：http://hz.cdnleiting.top/gtizzwfvjp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ybcxt.top/gtgftjqqyi.html

[T11] Kotlin：协程
来源：http://hz.jinghuilouyu.cn/gtflpsuwxu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinghuilouyu.cn/gtqmkgugnn.html

[T12] Kotlin：解构声明
来源：http://hz.ywan-chungtsiang.top/gtupqehrax.html

val (a, b) = Pair(1, 2)
来源：http://hz.gaohongyu789.top/gtcirjzabm.html

[T13] Kotlin：只读 Map
来源：http://hz.zhiwuduotai.top/gttzpuioxo.html

val m = mapOf("a" to 1)
来源：http://hz.gogol.net.cn/gtamfrimhb.html

[T14] Kotlin：循环
来源：http://hz.52xcode.cn/gtdbgovzrv.html

for (i in 1..10) println(i)
来源：http://hz.sysykeji.top/gtfzgnhbbn.html

[T15] Kotlin：接口
来源：http://hz.birdmap.top/gtpqintmnu.html

interface Shape { fun area(): Double }
来源：http://hz.sweek.top/gtiqfvcsia.html

[T16] Swift：Hello World
来源：http://hz.fzhhl.top/gtnyqdwzii.html

print("Hello")
来源：http://hz.hfpthk.cn/gtegdvaoiq.html

[T17] Swift：变量与常量
来源：http://hz.aibaodan.cn/gtyrectnrm.html

var a = 1;  let b = 2
来源：http://hz.hnxiangtu.top/gtibywdmue.html

[T18] Swift：字符串插值
来源：http://hz.yueranfly.top/gtgcqzzbre.html

"值: \(b)"
来源：http://hz.andypj.xyz/gtmcwdedew.html

[T19] Swift：可选绑定
来源：http://hz.yj20258888.top/gtbhgxqgyy.html

if let n = opt { print(n) }
来源：http://hz.yonumen.top/gtwcxiplpd.html

[T20] Swift：数组操作
来源：http://hz.zhiwuduotai.top/gtoywdwvhb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigufen.top/gttzgvxndm.html

[T21] Swift：遍历
来源：http://hz.xingfuxueyuan.xyz/gtxuhismhl.html

for x in a { print(x) }
来源：http://hz.guowangkeji.top/gthitenkak.html

[T22] Swift：字典
来源：http://hz.jiagoushi.top/gtrsufifxt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnqzz.top/gtgsygowlr.html

[T23] Swift：函数
来源：http://hz.guowangkeji.top/gtbavmwshk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shzxlz.cn/gtiaksuadc.html

[T24] Swift：闭包
来源：http://hz.ppjwa.cn/gtyberfwwe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.pengpengdd.cyou/gtpaiswufh.html

[T25] Swift：结构体
来源：http://hz.gotoacloud.top/gtiranxcej.html

struct P { var x: Int }
来源：http://hz.fengsongda.top/gtilwbsqww.html

[T26] Swift：类与重写
来源：http://hz.aibaodan.cn/gtfdtecznd.html

class A: Base { override func f() {} }
来源：http://hz.guannengcc.top/gtcpecswph.html

[T27] Swift：错误处理
来源：http://hz.shzxlz.cn/gtcznxisoo.html

do { try f() } catch { print(error) }
来源：http://hz.gotoacloud.top/gtpsqqqikj.html

[T28] Swift：枚举
来源：http://hz.ydzc1.top/gtpupxykdy.html

enum Color { case red, green }
来源：http://hz.mhx1999.top/gtbrhszuvz.html

[T29] Swift：guard 提前返回
来源：http://hz.yangfankeji.com/gtcygankqw.html

guard let x = opt else { return }
来源：http://hz.hywenlv.cn/gtggaciqgy.html

[T30] Swift：协议
来源：http://hz.haohaochexian.top/gtxqanapuj.html

protocol Shape { func area() -> Double }
来源：http://hz.yuanzhike.top/gtshvrlcrp.html

[T31] Lua：Hello World
来源：http://hz.hnqzz.top/gtaxnjhpbk.html

print("Hello")
来源：http://hz.xziqi.cn/gtsoqmhnud.html

[T32] Lua：局部变量
来源：http://hz.jlsjyb.cn/gtkqdsdswa.html

local a = 1
来源：http://hz.gogol.net.cn/gtipzchgvp.html

[T33] Lua：表（数组）
来源：http://hz.yj202588.top/gtohhybaeq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sxryk.cn/gtwohxilzz.html

[T34] Lua：遍历表
来源：http://hz.yonumen.top/gtgcimyryg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ybcxt.top/gtcujgpqqv.html

[T35] Lua：字典表
来源：http://hz.ydjk.org.cn/gtpuliqaup.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinyuanbaomall.cn/gtcuwylhog.html

[T36] Lua：函数
来源：http://hz.yj20258888.top/gtcdawpxxt.html

function add(a, b) return a + b end
来源：http://hz.hongshengwenyu.top/gtiaexkejn.html

[T37] Lua：字符串拼接
来源：http://hz.cheryme.top/gtsikkeuqs.html

"a" .. "b"
来源：http://hz.nwbrower.top/gtvupubutl.html

[T38] Lua：条件
来源：http://hz.yj20258888.top/gtaqgqarhj.html

if x > 0 then print("正") end
来源：http://hz.vqdsnc.cn/gtyfxwyqkd.html

[T39] Lua：模式匹配
来源：http://hz.vqdsnc.cn/gtsaqpxmhd.html

string.find(s, "%d+")
来源：http://hz.guannengcc.top/gtpihgrmdc.html

[T40] Lua：元表
来源：http://hz.316326.xyz/gtwegwwlsp.html

setmetatable({}, { __index = base })
来源：http://hz.sxryk.cn/gtdehdwvkl.html

[T41] Perl：Hello World
来源：http://hz.shangyingyoupin.top/gtnokcdzfp.html

print "Hello\n";
来源：http://hz.daria6918.cn/gtphtzebtk.html

[T42] Perl：变量类型
来源：http://hz.xziqi.cn/gthymuxfma.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hongshengwenyu.top/gtpaojzmwk.html

[T43] Perl：字符串插值
来源：http://hz.ivvv.top/gtghsguiln.html

"值: $a"
来源：http://hz.cashguo.top/gtllmcbjwc.html

[T44] Perl：条件
来源：http://hz.9152youxi.cn/gthxkonevt.html

if ($a > 0) { print "正"; }
来源：http://hz.jqgfzy.top/gtrlyjbikw.html

[T45] Perl：数组遍历
来源：http://hz.shuidangran.top/gtyqylrzym.html

for my $x (@arr) { print $x; }
来源：http://hz.chenzaomai.com/gtofkupfuo.html

[T46] Perl：哈希操作
来源：http://hz.ppjwa.cn/gtsxntvcna.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xziqi.cn/gtkazitgst.html

[T47] Perl：正则捕获
来源：http://hz.nanxuanxn.top/gtkxlhbxss.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gogol.net.cn/gteklzfbzi.html

[T48] Perl：正则替换
来源：http://hz.hnqzz.top/gtwnqsugwf.html

$s =~ s/old/new/g;
来源：http://hz.wangdashe.top/gtxyrbgvgh.html

[T49] Perl：函数
来源：http://hz.dianchejie.cn/gtejmizmis.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.0kj1m.cn/gtlkgftagg.html

[T50] Perl：逐行读文件
来源：http://hz.iojbl.cn/gtevncgxlc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.52xcode.cn/gtdndrhzmy.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.guannengcc.top/gttlvberhp.html

[T51] Scala：Hello World
来源：http://hz.yueranfly.top/gtxlopqdjp.html

println("Hello")
来源：http://hz.0kj1m.cn/gtijzzklki.html

[T52] Scala：变量
来源：http://hz.yj20258888.top/gtehrkpmgt.html

val a = 1;  var b = 2
来源：http://hz.yj202588.top/gtiujsrsgb.html

[T53] Scala：字符串插值
来源：http://hz.ybcxt.top/gtnemnvodb.html

s"值: $b"
来源：http://hz.hammf.cn/gtdsbysnhc.html

[T54] Scala：集合映射
来源：http://hz.jinghuilouyu.cn/gttuitfkbf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xuanzx.com/gthwgbtuus.html

[T55] Scala：集合过滤
来源：http://hz.ydjk.org.cn/gtztgkdque.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yueranfly.top/gtmagppjbh.html

[T56] Scala：样例类
来源：http://hz.cashguo.top/gtsepnbvse.html

case class User(name: String, age: Int)
来源：http://hz.ywan-chungtsiang.top/gtajrxarkp.html

[T57] Scala：模式匹配
来源：http://hz.chenlongwang.top/gtchjlzxya.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ybcxt.top/gtoivvbexl.html

[T58] Scala：函数定义
来源：http://hz.haohaochexian.top/gtyoegxamb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.feifeiyinyue.top/gthmhptsza.html

[T59] Scala：循环
来源：http://hz.zycfv.cn/gtingcxjcn.html

for (i <- 1 to 10) println(i)
来源：http://hz.hywenlv.cn/gtmmksquwg.html

[T60] Scala：折叠
来源：http://hz.xuanzx.com/gtvbzwauzv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yuanzhike.top/gttnzicykw.html

================================================================================
来源：http://hz.shuidangran.top/gttcpkpjmn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cucudq.cn/gtmrijlzam.html

================================================================================
来源：http://hz.andypj.xyz/gtxuiurdkv.html

[U01] Py：创建虚拟环境
来源：http://hz.wangdashe.top/gtudkcvttc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhiwuduotai.top/gtbghjhhjy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shzxlz.cn/gttcnuivpb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.dianchejie.cn/gtuohuljgw.html

[U03] Py：加载 .env 配置
来源：http://hz.feifeiyinyue.top/gthpejelta.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.dashuyun.cn/gtuujbifgb.html

[U04] Py：变量调试打印
来源：http://hz.9152youxi.cn/gtjjvtroqs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhiwuduotai.top/gtbgtscnor.html

[U05] Py：列表去重且保序
来源：http://hz.tanke756.top/gtjyqywrym.html

list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gttshqygjg.html

[U06] Py：合并两个字典
来源：http://hz.xuetiantiany.cn/gtadywafqd.html

{**a, **b}
来源：http://hz.yvedp.cn/gtrasmitxp.html

[U07] Py：反转字典键值
来源：http://hz.ydzc1.top/gthvxucboo.html

{v: k for k, v in d.items()}
来源：http://hz.9152youxi.cn/gtbpoczvqn.html

[U08] Py：展平二维列表
来源：http://hz.nanxinkj.top/gtxnqfmqfi.html

[y for x in nested for y in x]
来源：http://hz.jinyuanbaomall.cn/gtobctrrju.html

[U09] Py：字典取最大值的键
来源：http://hz.hnxiangtu.top/gttqbtwaeg.html

max(d, key=d.get)
来源：http://hz.hfpthk.cn/gtqvjbmniq.html

[U10] Py：按值排序字典
来源：http://hz.yuxming.cn/gtwwsdafwa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.0kj1m.cn/gthgeqddnf.html

[U11] Py：生成器表达式
来源：http://hz.yanxiufei.cn/gtnfjkfzrh.html

(x * 2 for x in arr)
来源：http://hz.iojbl.cn/gtfwtgpzev.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shanyushiyangkeji.top/gtcbamambo.html

Counter(arr).most_common(3)
来源：http://hz.yangfankeji.com/gtvqgtsdik.html

[U13] Py：固定长度队列
来源：http://hz.zhixingplan.top/gtaqtqgxmj.html

deque(maxlen=10)
来源：http://hz.yongpay.top/gtfthipfdg.html

[U14] Py：分组收集到列表
来源：http://hz.ehwqpu.com/gtpessmpbw.html

defaultdict(list)
来源：http://hz.xziqi.cn/gtbuogjdov.html

[U15] Py：高精度计时
来源：http://hz.ywan-chungtsiang.top/gtfjrjimbn.html

t = time.perf_counter()
来源：http://hz.316326.xyz/gtpowyhcds.html

[U16] Py：命令行参数解析
来源：http://hz.cdnleiting.top/gtbuwaudnt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.fengsongda.top/gtamkihsex.html

[U17] Py：初始化日志
来源：http://hz.ppjwa.cn/gtxnmbntqj.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shangyingyoupin.top/gtjnsuatlp.html

[U18] Py：预编译正则
来源：http://hz.xziqi.cn/gtfejkeqdn.html

pat = re.compile(r"\d+")
来源：http://hz.meibo888.top/gtyugpcmij.html

[U19] Py：正则替换带回调
来源：http://hz.hysaishi.cn/gtxesskmxb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhongyouzk.top/gtcfauslph.html

[U20] Py：缓存函数结果
来源：http://hz.wangshuangyany.cn/gthvgickyg.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ywan-chungtsiang.top/gtkwuhcvtp.html

[U21] Py：自定义上下文管理器
来源：http://hz.xuetiantiany.cn/gtjkmigsaz.html

@contextlib.contextmanager
来源：http://hz.jiagoushi.top/gtvecquvlv.html

[U22] Py：矩阵转置
来源：http://hz.havefunace.top/gtvtebbwqt.html

list(zip(*m))
来源：http://hz.wangshuangyany.cn/gtkadymaoe.html

[U23] Py：分块读取大文件
来源：http://hz.cucudq.cn/gtzbwyvrvu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.tian-w.cn/gtuffwbjdi.html

[U24] Py：路径操作
来源：http://hz.zhoulong.xyz/gtnvrubnay.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shanyushiyangtech.top/gtgmvjonpr.html

[U25] Py：CSV 按字典读
来源：http://hz.daria6918.cn/gtcumvmwpd.html

csv.DictReader(f)
来源：http://hz.chenlongwang.top/gtbexiitse.html

[U26] Py：并发下载
来源：http://hz.ybcxt.top/gtlhjyvxkf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ywan-chungtsiang.top/gtzdmwggwz.html

[U27] Py：异步 HTTP
来源：http://hz.sufxvd.cn/gtwizhwjcj.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cdnleiting.top/gtxamkcimy.html

[U28] Py：类型别名
来源：http://hz.hongshengwenyu.top/gtxnmyfnwn.html

UserId = int
来源：http://hz.haohaochexian.top/gtptmwices.html

[U29] Py：属性校验
来源：http://hz.zhaomingkeji.xyz/gtqjciinic.html

@property 与 @x.setter 配合
来源：http://hz.jqgfzy.top/gtwtrauujf.html

[U30] Py：数据类
来源：http://hz.yongpay.top/gtnpattbaw.html

@dataclass(slots=True)
来源：http://hz.hammf.cn/gtjuantvwo.html

[U31] Py：单测
来源：http://hz.zhiwuduotai.top/gtpvlcvrla.html

python -m pytest -q
来源：http://hz.yonumen.top/gtmhjgnoof.html

[U32] Py：代码格式化
来源：http://hz.guannengcc.top/gthwpuxnbb.html

ruff format . && ruff check --fix .
来源：http://hz.316326.xyz/gtxbbvktjd.html

[U33] Py：打包发布
来源：http://hz.fzhhl.top/gtikilwyna.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cqqwz.cn/gtppbcowuz.html

[U34] Py：判断编码
来源：http://hz.ppjwa.cn/gtjvoosacr.html

chardet.detect(raw)
来源：http://hz.ybcxt.top/gtdqmrsxnr.html

[U35] Py：发送邮件
来源：http://hz.tianlin.xyz/gtoxyehboh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.quarkkingdee.top/gtfiorjvog.html

[U36] Py：定时任务
来源：http://hz.yangfankeji.com/gtlkzwqmrw.html

schedule.every(10).minutes.do(job)
来源：http://hz.guannengcc.top/gtilcgfkal.html

[U37] Py：读写 Excel
来源：http://hz.ivvv.top/gtkhbevyph.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.52xcode.cn/gtrqjbpjqg.html

[U38] Py：获取脚本所在目录
来源：http://hz.hammf.cn/gtgywxceqs.html

Path(__file__).resolve().parent
来源：http://hz.zhongyouzk.top/gtjgtoesqs.html

[U39] Py：判断是否在交互环境
来源：http://hz.jinqigfzy.top/gtritpdnpe.html

sys.stdout.isatty()
来源：http://hz.chenjidiqi.icu/gtphvjajxj.html

[U40] Py：打印到标准错误
来源：http://hz.xuetiantiany.cn/gtisyqekyi.html

print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gtmvfyjgah.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sysykeji.top/gtefszxdhd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yongpay.top/gtpwgbhwkc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenzaomai.com/gtsbnnvzis.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.pycfn.com/gtgnayzvfd.html

[U43] PHP：声明命名空间
来源：http://hz.pycfn.com/gtivtekxjv.html

namespace App\Http;
来源：http://hz.shzxlz.cn/gtnkamxwji.html

[U44] PHP：开启严格类型
来源：http://hz.0kj1m.cn/gtexvlgupz.html

declare(strict_types=1);
来源：http://hz.mhx1999.top/gtablrppin.html

[U45] PHP：类型声明与返回类型
来源：http://hz.iojbl.cn/gtqbivzvqg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtxapwehgd.html

[U46] PHP：可空类型
来源：http://hz.shanyushiyangkeji.top/gtzawyxtvy.html

?string $name = null
来源：http://hz.zhixingplan.top/gtmfukirkg.html

[U47] PHP：联合类型
来源：http://hz.sysykeji.top/gtqasyjkvv.html

int|string $id
来源：http://hz.yangfankeji.com/gtsgqoviix.html

[U48] PHP：纯枚举
来源：http://hz.hysaishi.cn/gthdnnkxml.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ydzc1.top/gtxhmvacdc.html

[U49] PHP：只读属性
来源：http://hz.fengsongda.top/gtyozuosgj.html

public readonly string $name
来源：http://hz.bjfxy.top/gtcckknoiu.html

[U50] PHP：构造器属性提升
来源：http://hz.yj20258.top/gtohjghbni.html

public function __construct(private int $id) {}
来源：http://hz.nwbrower.top/gtawwaaipx.html

[U51] PHP：数组解构
来源：http://hz.xziqi.cn/gtbtoiganv.html

[$a, $b] = $arr;
来源：http://hz.bjfxy.top/gtralmnblh.html

[U52] PHP：箭头函数
来源：http://hz.316326.xyz/gtsotfikay.html

$double = fn($x) => $x * 2;
来源：http://hz.zhoulong.xyz/gtsnpvfrku.html

[U53] PHP：空合并运算符
来源：http://hz.cashguo.top/gtagznztia.html

$v = $a ?? $b ?? "default";
来源：http://hz.hnqzz.top/gtgsmjnozh.html

[U54] PHP：空安全调用
来源：http://hz.xuanzx.com/gtzrzhvprp.html

$obj?->method()
来源：http://hz.hysaishi.cn/gtvhyajfzj.html

[U55] PHP：match 表达式
来源：http://hz.vqdsnc.cn/gthweczyae.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.guannengcc.top/gtytnrxtcb.html

[U56] PHP：命名参数
来源：http://hz.havefunace.top/gtqlogwkoc.html

f(a: 1, b: 2)
来源：http://hz.ehwqpu.com/gtmpugwiwh.html

[U57] PHP：字符串插值
来源：http://hz.yanxiufei.cn/gtfyfzgipx.html

"值: {$a}"
来源：http://hz.sxryk.cn/gtngdnsutb.html

[U58] PHP：数组三件套
来源：http://hz.mhx1999.top/gteojagqau.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ppjwa.cn/gtuhhoygfv.html

[U59] PHP：自定义排序
来源：http://hz.haohaochexian.top/gtawbxmohl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yongpay.top/gtxizpwpun.html

[U60] PHP：JSON 编解码
来源：http://hz.yvedp.cn/gtiirwcnns.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.tanke756.top/gthvhlffxa.html

[U61] PHP：正则
来源：http://hz.guowangkeji.top/gtmdkwctjr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinyuanbaomall.cn/gtfrpwyxho.html

[U62] PHP：日期对象
来源：http://hz.sxryk.cn/gtlnvhswsq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.vqdsnc.cn/gtygmshitd.html

[U63] PHP：文件读写
来源：http://hz.jianghu66.top/gtxtzfumyy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.9152youxi.cn/gtvfuysnbw.html

[U64] PHP：目录遍历
来源：http://hz.smart0.xyz/gtylgnieek.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.0kj1m.cn/gtmtactsce.html

[U65] PHP：会话
来源：http://hz.xuetiantiany.cn/gtyaqqyqrx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.fzhhl.top/gtripmokev.html

[U66] PHP：设置 Cookie
来源：http://hz.ybcxt.top/gtrdvhmhsl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.vqdsnc.cn/gtaswuxidq.html

[U67] PHP：处理文件上传
来源：http://hz.iojbl.cn/gtpbsqrjzq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.kuanghao11.cn/gtrsdgozpz.html

[U68] PHP：PDO 连接
来源：http://hz.haohaochexian.top/gtxvregxwe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shanyushiyangtech.top/gtxgijfdvu.html

[U69] PHP：PDO 预处理
来源：http://hz.jqgufenzy.top/gtpnsajogf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xziqi.cn/gtvkukrgie.html

[U70] PHP：PDO 事务
来源：http://hz.jlsjyb.cn/gtobxwrxvj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yanxiufei.cn/gtpyuiyiej.html

[U71] PHP：抛出异常
来源：http://hz.yueranfly.top/gtfabtynxu.html

throw new RuntimeException("失败", 500);
来源：http://hz.vqdsnc.cn/gtfzzcsxdu.html

[U72] PHP：写错误日志
来源：http://hz.cashguo.top/gthiacalzx.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gzhubu.top/gtpiutaliy.html

[U73] PHP：读取 ini 配置
来源：http://hz.kuanghao11.cn/gtewhblmvs.html

parse_ini_file("config.ini", true)
来源：http://hz.yonumen.top/gtqzixalvp.html

[U74] PHP：读取环境变量
来源：http://hz.havefunace.top/gtunylrrlx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jinyuanbaomall.cn/gtqwqdkypv.html

[U75] PHP：依赖注入
来源：http://hz.haohaochexian.top/gtdqpcbggy.html

composer require psr/container
来源：http://hz.gogol.net.cn/gtrijdzrzl.html

[U76] PHP：简单路由
来源：http://hz.cqqwz.cn/gtdqgsriek.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.smart0.xyz/gtzkerxncc.html


<!-- 参考信息 -->