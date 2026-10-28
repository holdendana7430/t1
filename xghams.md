代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.52xcode.cn/gtewshpzlu.html

[S51] C++：显式类型转换
来源：http://hz.ydjk.org.cn/gtlhdqxjjw.html

static_cast<double>(a) / b
来源：http://hz.zhixingplan.top/gtxqfgshwd.html

[S52] C++：const 与 noexcept
来源：http://hz.mhx1999.top/gtajiwvdqv.html

int size() const noexcept { return n_; }
来源：http://hz.yongpay.top/gtghxffecg.html

[S53] C++：移动语义
来源：http://hz.chenlongwang.top/gtmhvwzhal.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258.top/gtkxknlhjs.html

[S54] C++：异常处理
来源：http://hz.zhaomingkeji.xyz/gtdkpvcwye.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guannengcc.top/gtlzcokrkb.html

[S55] C++：结构化绑定
来源：http://hz.smart0.xyz/gthwqfthrk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sxryk.cn/gtvkbsdewh.html

[S56] C++：optional
来源：http://hz.aibaodan.cn/gtwuyjnnum.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yuanzhike.top/gtweyzevum.html

[S57] C++：编译期常量
来源：http://hz.chenlongwang.top/gtndhxwqsv.html

constexpr int N = 10;
来源：http://hz.jlsjyb.cn/gtyeoqgnqb.html

[S58] C++：命名空间
来源：http://hz.yongpay.top/gtzbuekjhu.html

namespace ns { int f() { return 1; } }
来源：http://hz.xziqi.cn/gtrgepgmre.html

[S59] C++：静态断言
来源：http://hz.yongpay.top/gtnnviudmy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fengsongda.top/gtjnasmzxo.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangkeji.top/gtgkjtjfnw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.guowangkeji.top/gtxomgnbzr.html

================================================================================
来源：http://hz.zhoulong.xyz/gtsvhbxuzn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhiwuduotai.top/gtmiagjbts.html

================================================================================
来源：http://hz.ydjk.org.cn/gtlvnchhyr.html

[T01] Kotlin：Hello World
来源：http://hz.yuxming.cn/gtwagqbueg.html

println("Hello")
来源：http://hz.andypj.xyz/gthqqxamgk.html

[T02] Kotlin：变量
来源：http://hz.guowangkeji.top/gtgkuctmac.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.vqdsnc.cn/gtkktproxs.html

[T03] Kotlin：字符串模板
来源：http://hz.vqdsnc.cn/gticdiovab.html

"值: $b"
来源：http://hz.wangshuangyany.cn/gtdodfbpou.html

[T04] Kotlin：空安全
来源：http://hz.hnxiangtu.top/gtdoupjhkb.html

val n: String? = null;  n?.length
来源：http://hz.fengsongda.top/gtowbexnfi.html

[T05] Kotlin：when 表达式
来源：http://hz.cqqwz.cn/gtegcswjai.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cucudq.cn/gteucioknr.html

[T06] Kotlin：集合映射
来源：http://hz.sysykeji.top/gtplzfnxpm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yongpay.top/gtgzrxjwmi.html

[T07] Kotlin：集合过滤
来源：http://hz.chenzaomai.com/gtmdytvlnl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnxiangtu.top/gtnteinlgu.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangkeji.top/gtipfjvwxg.html

data class User(val name: String, val age: Int)
来源：http://hz.ydzc1.top/gtjvtdknls.html

[T09] Kotlin：扩展函数
来源：http://hz.kuanghao11.cn/gtgwqzqgoa.html

fun String.exclaim() = this + "!"
来源：http://hz.chenzaomai.com/gttxairult.html

[T10] Kotlin：默认参数
来源：http://hz.dianchejie.cn/gteeigqylk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cashguo.top/gtohnllbur.html

[T11] Kotlin：协程
来源：http://hz.yueranfly.top/gtrfljdcnr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gogol.net.cn/gtexxzraox.html

[T12] Kotlin：解构声明
来源：http://hz.svipenyu.cn/gtgbouiayf.html

val (a, b) = Pair(1, 2)
来源：http://hz.cqqwz.cn/gtvmjthqyo.html

[T13] Kotlin：只读 Map
来源：http://hz.pycfn.com/gtytvzvlsn.html

val m = mapOf("a" to 1)
来源：http://hz.wangdashe.top/gtedphfzii.html

[T14] Kotlin：循环
来源：http://hz.ydzc1.top/gtpsviqqlq.html

for (i in 1..10) println(i)
来源：http://hz.hywenlv.cn/gtnkozredi.html

[T15] Kotlin：接口
来源：http://hz.redwolf501.top/gtbhaodzuv.html

interface Shape { fun area(): Double }
来源：http://hz.jinqigufen.top/gtfffnlkgb.html

[T16] Swift：Hello World
来源：http://hz.yonumen.top/gttvjvsuhe.html

print("Hello")
来源：http://hz.zycfv.cn/gtprjkhluz.html

[T17] Swift：变量与常量
来源：http://hz.xuanzx.com/gtmzpagvdx.html

var a = 1;  let b = 2
来源：http://hz.nwbrower.top/gtmyexjtrd.html

[T18] Swift：字符串插值
来源：http://hz.tian-w.cn/gtrjacyocm.html

"值: \(b)"
来源：http://hz.vqdsnc.cn/gtqalbrzyu.html

[T19] Swift：可选绑定
来源：http://hz.tanke756.top/gthmegxgsd.html

if let n = opt { print(n) }
来源：http://hz.gzhubu.top/gtzaqdpxax.html

[T20] Swift：数组操作
来源：http://hz.yonumen.top/gtdgccpgqr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jyoumei.cn/gtnzopddlz.html

[T21] Swift：遍历
来源：http://hz.gzhubu.top/gtdzrrqihr.html

for x in a { print(x) }
来源：http://hz.hnqzz.top/gttwcwbdol.html

[T22] Swift：字典
来源：http://hz.snrcjt.cn/gtojbrgvtt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xylfe.cn/gtowhplnfj.html

[T23] Swift：函数
来源：http://hz.cqqwz.cn/gtfmtgmuvp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.smart0.xyz/gtrfgilejq.html

[T24] Swift：闭包
来源：http://hz.cucudq.cn/gtvcblcljs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.birdmap.top/gtxtnifels.html

[T25] Swift：结构体
来源：http://hz.yanxiufei.cn/gtlhkswykb.html

struct P { var x: Int }
来源：http://hz.gotoacloud.top/gtaxfirokx.html

[T26] Swift：类与重写
来源：http://hz.bjfxy.top/gtfvhwaqzq.html

class A: Base { override func f() {} }
来源：http://hz.iojbl.cn/gtuvuhscza.html

[T27] Swift：错误处理
来源：http://hz.cheryme.top/gtukhbgznv.html

do { try f() } catch { print(error) }
来源：http://hz.jiagoushi.top/gteqakklwg.html

[T28] Swift：枚举
来源：http://hz.zhengqikj.top/gtwmaffaaa.html

enum Color { case red, green }
来源：http://hz.yj202588.top/gtdjzkqkau.html

[T29] Swift：guard 提前返回
来源：http://hz.hongshengwenyu.top/gtywfcyytc.html

guard let x = opt else { return }
来源：http://hz.zhijiandao.cn/gtvogbufcb.html

[T30] Swift：协议
来源：http://hz.ydzc1.top/gthfxqsbzj.html

protocol Shape { func area() -> Double }
来源：http://hz.yongpay.top/gtxxzeclpq.html

[T31] Lua：Hello World
来源：http://hz.gotoacloud.top/gtgergwgex.html

print("Hello")
来源：http://hz.kuanghao11.cn/gtmmropcpa.html

[T32] Lua：局部变量
来源：http://hz.xziqi.cn/gtbrmmnevb.html

local a = 1
来源：http://hz.zdqjudy.top/gtcduauarp.html

[T33] Lua：表（数组）
来源：http://hz.xuetiantiany.cn/gtczzuljlv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shuidangran.top/gtmvdgxoqg.html

[T34] Lua：遍历表
来源：http://hz.jlsjyb.cn/gtolakqunz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.9152youxi.cn/gtxoxgfzgw.html

[T35] Lua：字典表
来源：http://hz.ppjwa.cn/gtbkygfcrn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sxryk.cn/gtdajvebiu.html

[T36] Lua：函数
来源：http://hz.daxiang520.top/gtzjotrxvw.html

function add(a, b) return a + b end
来源：http://hz.feifeiyinyue.top/gttnmfuqjj.html

[T37] Lua：字符串拼接
来源：http://hz.hfpthk.cn/gtnzduudhj.html

"a" .. "b"
来源：http://hz.bjfxy.top/gtyevspyes.html

[T38] Lua：条件
来源：http://hz.zhongyouzk.top/gtpyrsxeij.html

if x > 0 then print("正") end
来源：http://hz.jianghu66.top/gtbsclmiko.html

[T39] Lua：模式匹配
来源：http://hz.jqgufenzy.top/gttofiehkf.html

string.find(s, "%d+")
来源：http://hz.cdnleiting.top/gtukeuyuoa.html

[T40] Lua：元表
来源：http://hz.daria6918.cn/gtdevwyofm.html

setmetatable({}, { __index = base })
来源：http://hz.jqgfzy.top/gtblbbjisj.html

[T41] Perl：Hello World
来源：http://hz.0kj1m.cn/gtjxkgchnr.html

print "Hello\n";
来源：http://hz.gogol.net.cn/gtfcrupdaj.html

[T42] Perl：变量类型
来源：http://hz.aibaodan.cn/gtacpwehuk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhoulong.xyz/gtbghpphrq.html

[T43] Perl：字符串插值
来源：http://hz.yueranfly.top/gtcjoiapxw.html

"值: $a"
来源：http://hz.ivvv.top/gtaqkvoutv.html

[T44] Perl：条件
来源：http://hz.jlsjyb.cn/gtxalckyca.html

if ($a > 0) { print "正"; }
来源：http://hz.yuxming.cn/gtlkahdsys.html

[T45] Perl：数组遍历
来源：http://hz.svipenyu.cn/gtsyymrljj.html

for my $x (@arr) { print $x; }
来源：http://hz.hnqzz.top/gtdthvnyaz.html

[T46] Perl：哈希操作
来源：http://hz.chenlongwang.top/gtobjdzrdm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.bjfxy.top/gtlufntypp.html

[T47] Perl：正则捕获
来源：http://hz.hysaishi.cn/gtxertqyuf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.wangshuangyany.cn/gtnewuxekf.html

[T48] Perl：正则替换
来源：http://hz.yj20258888.top/gtsmhtjadw.html

$s =~ s/old/new/g;
来源：http://hz.jyoumei.cn/gtiywqmbfn.html

[T49] Perl：函数
来源：http://hz.vqdsnc.cn/gtrpymbslu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sufxvd.cn/gtyooagyqh.html

[T50] Perl：逐行读文件
来源：http://hz.jinqigfzy.top/gtmceahhzv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ydzc1.top/gtygrbuanz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.9152youxi.cn/gtbktxfkwu.html

[T51] Scala：Hello World
来源：http://hz.cdnleiting.top/gtoevkafyz.html

println("Hello")
来源：http://hz.hnxiangtu.top/gtgmqbjonx.html

[T52] Scala：变量
来源：http://hz.zhixingplan.top/gtizhvzxdq.html

val a = 1;  var b = 2
来源：http://hz.shzxlz.cn/gtnknelvna.html

[T53] Scala：字符串插值
来源：http://hz.feifeiyinyue.top/gtuurovfxy.html

s"值: $b"
来源：http://hz.tianlin.xyz/gtkndkavhe.html

[T54] Scala：集合映射
来源：http://hz.yuxming.cn/gtfeopftpl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.snrcjt.cn/gtgkawfipb.html

[T55] Scala：集合过滤
来源：http://hz.xuetiantiany.cn/gtbhdmqsum.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yj202588.top/gtuwxhuejy.html

[T56] Scala：样例类
来源：http://hz.meibo888.top/gtnpxicyey.html

case class User(name: String, age: Int)
来源：http://hz.9152youxi.cn/gtxpkvvqha.html

[T57] Scala：模式匹配
来源：http://hz.gotoacloud.top/gtxbivfnle.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhiwuduotai.top/gtexpsxmgb.html

[T58] Scala：函数定义
来源：http://hz.c1oappe.top/gtkviliykz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenjidiqi.icu/gtjokddpjb.html

[T59] Scala：循环
来源：http://hz.chenlongwang.top/gtzllzjziv.html

for (i <- 1 to 10) println(i)
来源：http://hz.ivvv.top/gtvimtgyip.html

[T60] Scala：折叠
来源：http://hz.fengsongda.top/gtrnabeuhq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhongyouzk.top/gtqwklewsl.html

================================================================================
来源：http://hz.daxiang520.top/gtvzbjezvh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.kuanghao11.cn/gtuairfpwo.html

================================================================================
来源：http://hz.yonumen.top/gtbavmiaee.html

[U01] Py：创建虚拟环境
来源：http://hz.feifeiyinyue.top/gtelkefgvz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hammf.cn/gtfiqqzjxc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jqgfzy.top/gtymcypszx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.wangshuangyany.cn/gtjqptnvgq.html

[U03] Py：加载 .env 配置
来源：http://hz.daria6918.cn/gtgayyngzj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ivvv.top/gtxvvyhvzt.html

[U04] Py：变量调试打印
来源：http://hz.xuanzx.com/gtillorlpb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zycfv.cn/gturgamxgc.html

[U05] Py：列表去重且保序
来源：http://hz.shangyingyoupin.top/gtsclefdun.html

list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtrtoaxrnx.html

[U06] Py：合并两个字典
来源：http://hz.zhixingplan.top/gtkljvthvl.html

{**a, **b}
来源：http://hz.zhongyouzk.top/gtkspipowa.html

[U07] Py：反转字典键值
来源：http://hz.ivvv.top/gthhrvlona.html

{v: k for k, v in d.items()}
来源：http://hz.chenlongwang.top/gtxjxcbsqh.html

[U08] Py：展平二维列表
来源：http://hz.chenzaomai.com/gtityzhgrx.html

[y for x in nested for y in x]
来源：http://hz.smart0.xyz/gtanyobknf.html

[U09] Py：字典取最大值的键
来源：http://hz.sufxvd.cn/gtknbvrziu.html

max(d, key=d.get)
来源：http://hz.chenlongwang.top/gthcodqlre.html

[U10] Py：按值排序字典
来源：http://hz.ppjwa.cn/gthjepmjox.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cucudq.cn/gtsezuufxk.html

[U11] Py：生成器表达式
来源：http://hz.kuanghao11.cn/gtmjyemjky.html

(x * 2 for x in arr)
来源：http://hz.ppjwa.cn/gtovvazfmd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hfpthk.cn/gtlcdwcasr.html

Counter(arr).most_common(3)
来源：http://hz.chenzaomai.com/gtnnqqdwsf.html

[U13] Py：固定长度队列
来源：http://hz.pycfn.com/gtbzxhqcfx.html

deque(maxlen=10)
来源：http://hz.cqqwz.cn/gtcziyfngg.html

[U14] Py：分组收集到列表
来源：http://hz.pengpengdd.cyou/gtlmpsgwnx.html

defaultdict(list)
来源：http://hz.xuanzx.com/gtxjqhwgmz.html

[U15] Py：高精度计时
来源：http://hz.cucudq.cn/gtgbrmuybu.html

t = time.perf_counter()
来源：http://hz.yj202588.top/gtjmkoizrp.html

[U16] Py：命令行参数解析
来源：http://hz.quarkkingdee.top/gtywhkhvki.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ydzc1.top/gtgpgezses.html

[U17] Py：初始化日志
来源：http://hz.xziqi.cn/gtehojpcyv.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yongpay.top/gtbakntuve.html

[U18] Py：预编译正则
来源：http://hz.yj20258888.top/gtypjsclrm.html

pat = re.compile(r"\d+")
来源：http://hz.hnqzz.top/gttjptogyf.html

[U19] Py：正则替换带回调
来源：http://hz.yongpay.top/gtvgfvmbhy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hammf.cn/gtcqjisfpc.html

[U20] Py：缓存函数结果
来源：http://hz.yuanzhike.top/gtcjilazkw.html

@functools.lru_cache(maxsize=None)
来源：http://hz.nwbrower.top/gtwqoenlik.html

[U21] Py：自定义上下文管理器
来源：http://hz.shangyingyoupin.top/gtosuusfsy.html

@contextlib.contextmanager
来源：http://hz.chenlongwang.top/gtostsljdo.html

[U22] Py：矩阵转置
来源：http://hz.aibaodan.cn/gttrnppcln.html

list(zip(*m))
来源：http://hz.jyoumei.cn/gtnkdyazro.html

[U23] Py：分块读取大文件
来源：http://hz.ehwqpu.com/gtcgrqkasq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zycfv.cn/gtvworkynh.html

[U24] Py：路径操作
来源：http://hz.chenlongwang.top/gtyzrsthqn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.nwbrower.top/gtbdfqayqy.html

[U25] Py：CSV 按字典读
来源：http://hz.havefunace.top/gtzxscnhwh.html

csv.DictReader(f)
来源：http://hz.ppjwa.cn/gtdaouzhzj.html

[U26] Py：并发下载
来源：http://hz.jqgufenzy.top/gtjrbqpsna.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shangyingyoupin.top/gtelysebhr.html

[U27] Py：异步 HTTP
来源：http://hz.yj202588.top/gtaixandko.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.316326.xyz/gtnlmxttvy.html

[U28] Py：类型别名
来源：http://hz.nanxinkj.top/gtthproycf.html

UserId = int
来源：http://hz.hysaishi.cn/gtnqivgorj.html

[U29] Py：属性校验
来源：http://hz.zdqjudy.top/gtkavmizub.html

@property 与 @x.setter 配合
来源：http://hz.bjfxy.top/gtmfuzslne.html

[U30] Py：数据类
来源：http://hz.feifeiyinyue.top/gtcdzzhoio.html

@dataclass(slots=True)
来源：http://hz.wangdashe.top/gtrovgrbpj.html

[U31] Py：单测
来源：http://hz.jianghu66.top/gtgtzugons.html

python -m pytest -q
来源：http://hz.wangdashe.top/gtrdgktdew.html

[U32] Py：代码格式化
来源：http://hz.yuanzhike.top/gtfrtlybnm.html

ruff format . && ruff check --fix .
来源：http://hz.xinyue.icu/gtzregunxi.html

[U33] Py：打包发布
来源：http://hz.0kj1m.cn/gtujaaqldu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yj202588.top/gttqekyfnt.html

[U34] Py：判断编码
来源：http://hz.tianlin.xyz/gtwjuttgfw.html

chardet.detect(raw)
来源：http://hz.ydzc1.top/gtvozcbhdr.html

[U35] Py：发送邮件
来源：http://hz.yonumen.top/gttfghhlno.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shanyushiyangtech.top/gtqmgtidiv.html

[U36] Py：定时任务
来源：http://hz.hywenlv.cn/gtbhdkwbho.html

schedule.every(10).minutes.do(job)
来源：http://hz.dashuyun.cn/gtibfuukhf.html

[U37] Py：读写 Excel
来源：http://hz.yanxiufei.cn/gttuwmechd.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xziqi.cn/gtxszhsggf.html

[U38] Py：获取脚本所在目录
来源：http://hz.xuanzx.com/gtlynatkqf.html

Path(__file__).resolve().parent
来源：http://hz.shuidangran.top/gtgrmdlyqe.html

[U39] Py：判断是否在交互环境
来源：http://hz.haohaochexian.top/gtijschdvf.html

sys.stdout.isatty()
来源：http://hz.jqgufenzy.top/gtovzqqilh.html

[U40] Py：打印到标准错误
来源：http://hz.0kj1m.cn/gthumkhjvj.html

print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtwfyudpps.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenlongwang.top/gtvyfvsimk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.aibaodan.cn/gtqtwhnhtt.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xinyue.icu/gtbwydfhcl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zycfv.cn/gteaisftkk.html

[U43] PHP：声明命名空间
来源：http://hz.tianlin.xyz/gthsspxpvt.html

namespace App\Http;
来源：http://hz.cheryme.top/gtyiclmadq.html

[U44] PHP：开启严格类型
来源：http://hz.hysaishi.cn/gtmbfudcdw.html

declare(strict_types=1);
来源：http://hz.jianghu66.top/gtczwaowmf.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yuxming.cn/gtzohkbocm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gtljixxven.html

[U46] PHP：可空类型
来源：http://hz.shanyushiyangtech.top/gtxospgtka.html

?string $name = null
来源：http://hz.gotoacloud.top/gtripsfwzh.html

[U47] PHP：联合类型
来源：http://hz.jinghuilouyu.cn/gtyfifkidt.html

int|string $id
来源：http://hz.snrcjt.cn/gtffpwcahm.html

[U48] PHP：纯枚举
来源：http://hz.yj202588.top/gthrysuddl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.nanxinkj.top/gtwdkiavsb.html

[U49] PHP：只读属性
来源：http://hz.vqdsnc.cn/gtpuhystsu.html

public readonly string $name
来源：http://hz.xylfe.cn/gtedxbsxrx.html

[U50] PHP：构造器属性提升
来源：http://hz.quarkkingdee.top/gtfnextukj.html

public function __construct(private int $id) {}
来源：http://hz.wangshuangyany.cn/gtwygbvqzz.html

[U51] PHP：数组解构
来源：http://hz.guannengcc.top/gtfjbassoe.html

[$a, $b] = $arr;
来源：http://hz.hammf.cn/gtzyudoslf.html

[U52] PHP：箭头函数
来源：http://hz.jqgfzy.top/gtvwpizihl.html

$double = fn($x) => $x * 2;
来源：http://hz.iojbl.cn/gtcxrascfc.html

[U53] PHP：空合并运算符
来源：http://hz.nwbrower.top/gtkaxxqjst.html

$v = $a ?? $b ?? "default";
来源：http://hz.ydzc1.top/gtfpseudil.html

[U54] PHP：空安全调用
来源：http://hz.shanyushiyangkeji.top/gtzazrxmqq.html

$obj?->method()
来源：http://hz.yuanzhike.top/gtmkrxurmr.html

[U55] PHP：match 表达式
来源：http://hz.xuetiantiany.cn/gtpwnhtxcs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.kuanghao11.cn/gtakfyrjus.html

[U56] PHP：命名参数
来源：http://hz.cdnleiting.top/gtmgvxgegr.html

f(a: 1, b: 2)
来源：http://hz.cqqwz.cn/gttwjjkick.html

[U57] PHP：字符串插值
来源：http://hz.sxryk.cn/gtxmsehytk.html

"值: {$a}"
来源：http://hz.shanyushiyangtech.top/gtdwpygrsn.html

[U58] PHP：数组三件套
来源：http://hz.jinghuilouyu.cn/gtuieezrex.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xingfuxueyuan.xyz/gtlbryftbp.html

[U59] PHP：自定义排序
来源：http://hz.jqgufenzy.top/gtyiubehlo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ehwqpu.com/gtdokfyzpk.html

[U60] PHP：JSON 编解码
来源：http://hz.meibo888.top/gtfhfndwmy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xylfe.cn/gtejywigna.html

[U61] PHP：正则
来源：http://hz.xuetiantiany.cn/gtpmhxfchw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhijiandao.cn/gtddrigpnk.html

[U62] PHP：日期对象
来源：http://hz.pengpengdd.cyou/gtzjdragam.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhaomingkeji.xyz/gtbqactncu.html

[U63] PHP：文件读写
来源：http://hz.jianghu66.top/gtrnuiuxaq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shzxlz.cn/gtkneibojh.html

[U64] PHP：目录遍历
来源：http://hz.cashguo.top/gtwrfhniiz.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hywenlv.cn/gtrqeabflo.html

[U65] PHP：会话
来源：http://hz.zdqjudy.top/gttorgwcrf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hfpthk.cn/gtioadfuym.html

[U66] PHP：设置 Cookie
来源：http://hz.sxryk.cn/gtvdpvdrbl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gaohongyu789.top/gtuilpzdin.html

[U67] PHP：处理文件上传
来源：http://hz.dashuyun.cn/gthwyvwjrg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zdqjudy.top/gtolndvpfx.html

[U68] PHP：PDO 连接
来源：http://hz.haohaochexian.top/gtluxvuvxf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.tian-w.cn/gtvjmabzun.html

[U69] PHP：PDO 预处理
来源：http://hz.0kj1m.cn/gtbndyvvzd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gotoacloud.top/gtrfzdsmnu.html

[U70] PHP：PDO 事务
来源：http://hz.redwolf501.top/gtzhctikjl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hnqzz.top/gtvjtuqzym.html

[U71] PHP：抛出异常
来源：http://hz.andypj.xyz/gtfnwqvids.html

throw new RuntimeException("失败", 500);
来源：http://hz.haohaochexian.top/gtnfszeiop.html

[U72] PHP：写错误日志
来源：http://hz.zhoulong.xyz/gtecugpowi.html

error_log("失败: " . $e->getMessage());
来源：http://hz.havefunace.top/gtzouhvoee.html

[U73] PHP：读取 ini 配置
来源：http://hz.xuanzx.com/gtyxazadda.html

parse_ini_file("config.ini", true)
来源：http://hz.meibo888.top/gtqztwluyo.html

[U74] PHP：读取环境变量
来源：http://hz.yuanzhike.top/gtjudxfpwx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hysaishi.cn/gtnvzrrucd.html

[U75] PHP：依赖注入
来源：http://hz.jqgufenzy.top/gtfxfrilso.html

composer require psr/container
来源：http://hz.redwolf501.top/gtrucyuqer.html

[U76] PHP：简单路由
来源：http://hz.cucudq.cn/gtscknurkr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hongshengwenyu.top/gtstbiorhk.html


<!-- 参考信息 -->