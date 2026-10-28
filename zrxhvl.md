代发 wailian999

int size() const noexcept { return n_; }
来源：http://hz.cdnleiting.top/gtmojgbchm.html

[S53] C++：移动语义
来源：http://hz.jinyuanbaomall.cn/gtyplnsnkd.html

std::vector<int> w = std::move(v);
来源：http://hz.hysaishi.cn/gtkbyrwjvt.html

[S54] C++：异常处理
来源：http://hz.zhijiandao.cn/gthvtwjoqn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.haohaochexian.top/gtokujpfyz.html

[S55] C++：结构化绑定
来源：http://hz.jqgfzy.top/gtajxpuvwk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuxming.cn/gtgnqvbhoc.html

[S56] C++：optional
来源：http://hz.cashguo.top/gtmjcburig.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gaohongyu789.top/gtbqysqfoq.html

[S57] C++：编译期常量
来源：http://hz.tanke756.top/gtutxkutru.html

constexpr int N = 10;
来源：http://hz.316326.xyz/gtxahwanff.html

[S58] C++：命名空间
来源：http://hz.yangfankeji.com/gtwiovwzdh.html

namespace ns { int f() { return 1; } }
来源：http://hz.shanyushiyangtech.top/gtqypuzbui.html

[S59] C++：静态断言
来源：http://hz.nanxinkj.top/gtphrmyowz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yueranfly.top/gterxdcypg.html

[S60] C++：遍历并删除元素
来源：http://hz.yvedp.cn/gtxcguonuf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhengqikj.top/gtflwmlykg.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtbmsiakxa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ywan-chungtsiang.top/gtuwjpvjvw.html

================================================================================
来源：http://hz.tianlin.xyz/gtaanptfmr.html

[T01] Kotlin：Hello World
来源：http://hz.hywenlv.cn/gtaonfdvzb.html

println("Hello")
来源：http://hz.quarkkingdee.top/gtiounxvum.html

[T02] Kotlin：变量
来源：http://hz.andypj.xyz/gtvwenwiaw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhongyouzk.top/gtxhzsvaer.html

[T03] Kotlin：字符串模板
来源：http://hz.shangyingyoupin.top/gtxguazaut.html

"值: $b"
来源：http://hz.jlsjyb.cn/gtwzcpgqfx.html

[T04] Kotlin：空安全
来源：http://hz.cdnleiting.top/gtjnxiqcyv.html

val n: String? = null;  n?.length
来源：http://hz.cdnleiting.top/gtgcpddqtj.html

[T05] Kotlin：when 表达式
来源：http://hz.shanyushiyangkeji.top/gtunjezhns.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.aibaodan.cn/gtwribkxht.html

[T06] Kotlin：集合映射
来源：http://hz.ppjwa.cn/gtdqhsylcv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xuanzx.com/gtdvjmbglx.html

[T07] Kotlin：集合过滤
来源：http://hz.mhx1999.top/gtmspgsgmm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shangyingyoupin.top/gtlhrmqqcg.html

[T08] Kotlin：数据类
来源：http://hz.hfpthk.cn/gtjjammwfi.html

data class User(val name: String, val age: Int)
来源：http://hz.pengpengdd.cyou/gtynoiuxzw.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgufenzy.top/gtnhmjvntf.html

fun String.exclaim() = this + "!"
来源：http://hz.zhiwuduotai.top/gtvejwjkzm.html

[T10] Kotlin：默认参数
来源：http://hz.jqgufenzy.top/gtwmgebbmu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.vqdsnc.cn/gtspnvixyg.html

[T11] Kotlin：协程
来源：http://hz.yanxiufei.cn/gtqrttsacs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daxiang520.top/gtonyrihcr.html

[T12] Kotlin：解构声明
来源：http://hz.daxiang520.top/gtjzldjrpb.html

val (a, b) = Pair(1, 2)
来源：http://hz.cucudq.cn/gtptzegxjs.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258.top/gtdnmvjafg.html

val m = mapOf("a" to 1)
来源：http://hz.aibaodan.cn/gtdmokuwmh.html

[T14] Kotlin：循环
来源：http://hz.pycfn.com/gtlhfigpti.html

for (i in 1..10) println(i)
来源：http://hz.shanyushiyangkeji.top/gtuupbbigw.html

[T15] Kotlin：接口
来源：http://hz.smart0.xyz/gtitqhgxko.html

interface Shape { fun area(): Double }
来源：http://hz.haohaochexian.top/gtemkoictf.html

[T16] Swift：Hello World
来源：http://hz.jlsjyb.cn/gteuttoxvc.html

print("Hello")
来源：http://hz.snrcjt.cn/gtablixqmh.html

[T17] Swift：变量与常量
来源：http://hz.hammf.cn/gtxyxssrmf.html

var a = 1;  let b = 2
来源：http://hz.daria6918.cn/gtzrdosxoc.html

[T18] Swift：字符串插值
来源：http://hz.ydzc1.top/gtolafufwk.html

"值: \(b)"
来源：http://hz.cheryme.top/gtrhvfdzfh.html

[T19] Swift：可选绑定
来源：http://hz.shuidangran.top/gtzarphunk.html

if let n = opt { print(n) }
来源：http://hz.zhengqikj.top/gtysiylpsk.html

[T20] Swift：数组操作
来源：http://hz.ybcxt.top/gthvuuctvo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.meibo888.top/gtjcclfptr.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gtphsuwkkv.html

for x in a { print(x) }
来源：http://hz.guowangkeji.top/gtdsprixeh.html

[T22] Swift：字典
来源：http://hz.hywenlv.cn/gtjzbnzslv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.wangdashe.top/gtfdwvcypp.html

[T23] Swift：函数
来源：http://hz.gogol.net.cn/gtxwryhswx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.quarkkingdee.top/gtnlerdqpt.html

[T24] Swift：闭包
来源：http://hz.9152youxi.cn/gtuvezpiib.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.daxiang520.top/gtnsgrhsgd.html

[T25] Swift：结构体
来源：http://hz.andypj.xyz/gtpzmpkemv.html

struct P { var x: Int }
来源：http://hz.hnqzz.top/gtcapsfllv.html

[T26] Swift：类与重写
来源：http://hz.snrcjt.cn/gtnunilrmr.html

class A: Base { override func f() {} }
来源：http://hz.xuetiantiany.cn/gtbtasnvlk.html

[T27] Swift：错误处理
来源：http://hz.wangshuangyany.cn/gtephylhus.html

do { try f() } catch { print(error) }
来源：http://hz.aibaodan.cn/gtsxaplqcl.html

[T28] Swift：枚举
来源：http://hz.ydjk.org.cn/gtnaslugys.html

enum Color { case red, green }
来源：http://hz.havefunace.top/gttihtobhx.html

[T29] Swift：guard 提前返回
来源：http://hz.yueranfly.top/gtkormhdbp.html

guard let x = opt else { return }
来源：http://hz.ehwqpu.com/gtxxqshcbn.html

[T30] Swift：协议
来源：http://hz.zycfv.cn/gtiqnrexgp.html

protocol Shape { func area() -> Double }
来源：http://hz.yj20258888.top/gtbpfxouep.html

[T31] Lua：Hello World
来源：http://hz.redwolf501.top/gtcpyfiipm.html

print("Hello")
来源：http://hz.shzxlz.cn/gtqqtqwkbv.html

[T32] Lua：局部变量
来源：http://hz.gogol.net.cn/gtlewjwirx.html

local a = 1
来源：http://hz.iojbl.cn/gtggbmnhug.html

[T33] Lua：表（数组）
来源：http://hz.tian-w.cn/gtvwdmqrhf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.iojbl.cn/gtkjgaluny.html

[T34] Lua：遍历表
来源：http://hz.zycfv.cn/gtlkitnptq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shanyushiyangkeji.top/gtohkdyazz.html

[T35] Lua：字典表
来源：http://hz.9152youxi.cn/gtswgmvsdx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cheryme.top/gtvyiosasl.html

[T36] Lua：函数
来源：http://hz.cashguo.top/gtmfvkrovh.html

function add(a, b) return a + b end
来源：http://hz.kuanghao11.cn/gtiheibqga.html

[T37] Lua：字符串拼接
来源：http://hz.gogol.net.cn/gtacmfjymq.html

"a" .. "b"
来源：http://hz.ppjwa.cn/gtsrazhswp.html

[T38] Lua：条件
来源：http://hz.shanyushiyangtech.top/gtchzhlcty.html

if x > 0 then print("正") end
来源：http://hz.9152youxi.cn/gttwfayrte.html

[T39] Lua：模式匹配
来源：http://hz.hnxiangtu.top/gtuwlyvgat.html

string.find(s, "%d+")
来源：http://hz.shanyushiyangkeji.top/gtshtfylyw.html

[T40] Lua：元表
来源：http://hz.nwbrower.top/gtmtikexmg.html

setmetatable({}, { __index = base })
来源：http://hz.guowangkeji.top/gtqkprlmob.html

[T41] Perl：Hello World
来源：http://hz.zycfv.cn/gtsevnwmgg.html

print "Hello\n";
来源：http://hz.nanxuanxn.top/gtoddyauuq.html

[T42] Perl：变量类型
来源：http://hz.hammf.cn/gtddvyuuig.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hfpthk.cn/gtvbxkuqjt.html

[T43] Perl：字符串插值
来源：http://hz.gaohongyu789.top/gtwbdlpfoq.html

"值: $a"
来源：http://hz.chenzaomai.com/gtnwmmrngr.html

[T44] Perl：条件
来源：http://hz.ivvv.top/gtvrpokchm.html

if ($a > 0) { print "正"; }
来源：http://hz.zhijiandao.cn/gtntfnlzey.html

[T45] Perl：数组遍历
来源：http://hz.guannengcc.top/gtvfakjaoh.html

for my $x (@arr) { print $x; }
来源：http://hz.sysykeji.top/gtezxytkun.html

[T46] Perl：哈希操作
来源：http://hz.nanxinkj.top/gtbvfjblud.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.snrcjt.cn/gtzffcukrj.html

[T47] Perl：正则捕获
来源：http://hz.zhengqikj.top/gtrmyrcitj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jiagoushi.top/gtuhwhspjl.html

[T48] Perl：正则替换
来源：http://hz.tianlin.xyz/gtpnucaozw.html

$s =~ s/old/new/g;
来源：http://hz.jinghuilouyu.cn/gtllulzmao.html

[T49] Perl：函数
来源：http://hz.feifeiyinyue.top/gtrszufncc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jiagoushi.top/gtbuboolxh.html

[T50] Perl：逐行读文件
来源：http://hz.daria6918.cn/gtusthapbp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ivvv.top/gtwpximgbe.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.sufxvd.cn/gtwbskcqos.html

[T51] Scala：Hello World
来源：http://hz.ehwqpu.com/gtsmwpqeqp.html

println("Hello")
来源：http://hz.feifeiyinyue.top/gtyrxkgxdn.html

[T52] Scala：变量
来源：http://hz.jqgfzy.top/gttaqdatnq.html

val a = 1;  var b = 2
来源：http://hz.jinghuilouyu.cn/gtuyqakyuv.html

[T53] Scala：字符串插值
来源：http://hz.guowangkeji.top/gtfqmtyjbx.html

s"值: $b"
来源：http://hz.guowangkeji.top/gtzvzuyogw.html

[T54] Scala：集合映射
来源：http://hz.cqqwz.cn/gtpsqaxbwp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hammf.cn/gtsdzvuqoi.html

[T55] Scala：集合过滤
来源：http://hz.jinqigufen.top/gtcymtgvvg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yangfankeji.com/gtauiqoohd.html

[T56] Scala：样例类
来源：http://hz.jinyuanbaomall.cn/gtpqcatgvc.html

case class User(name: String, age: Int)
来源：http://hz.mhx1999.top/gtsqjkzezf.html

[T57] Scala：模式匹配
来源：http://hz.pycfn.com/gtekqkkhdc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.haohaochexian.top/gtgnfgndpp.html

[T58] Scala：函数定义
来源：http://hz.haohaochexian.top/gtvtkscufo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sufxvd.cn/gtaphcrjrq.html

[T59] Scala：循环
来源：http://hz.feifeiyinyue.top/gtqyuocgwk.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhengqikj.top/gtlfaudvrv.html

[T60] Scala：折叠
来源：http://hz.52xcode.cn/gtcmegnzgq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.nwbrower.top/gtavzgrkyk.html

================================================================================
来源：http://hz.zhengqikj.top/gtdcixjbpz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.quarkkingdee.top/gtmxlpkcov.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtwewfqjiv.html

[U01] Py：创建虚拟环境
来源：http://hz.xylfe.cn/gtzessgpqd.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhijiandao.cn/gtabxonsvr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cheryme.top/gtrkdtdtvx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.tianlin.xyz/gtfbjqkwzj.html

[U03] Py：加载 .env 配置
来源：http://hz.jiagoushi.top/gtftjzjtmo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.wangshuangyany.cn/gtaqkvgeot.html

[U04] Py：变量调试打印
来源：http://hz.havefunace.top/gtckdbfyuj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.0kj1m.cn/gtlloflwfr.html

[U05] Py：列表去重且保序
来源：http://hz.cashguo.top/gttbqthrph.html

list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gtdllcptou.html

[U06] Py：合并两个字典
来源：http://hz.zhongyouzk.top/gtuvrlmfjj.html

{**a, **b}
来源：http://hz.ppjwa.cn/gtawdosqag.html

[U07] Py：反转字典键值
来源：http://hz.yongpay.top/gtxslpwgez.html

{v: k for k, v in d.items()}
来源：http://hz.yongpay.top/gtljuggcpq.html

[U08] Py：展平二维列表
来源：http://hz.ybcxt.top/gtvhpzcray.html

[y for x in nested for y in x]
来源：http://hz.ehwqpu.com/gtondtrgdg.html

[U09] Py：字典取最大值的键
来源：http://hz.ydzc1.top/gtxyfcbvqx.html

max(d, key=d.get)
来源：http://hz.cheryme.top/gtweiijpwp.html

[U10] Py：按值排序字典
来源：http://hz.nanxuanxn.top/gtdnkeldtr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.fengsongda.top/gtnbalrlvz.html

[U11] Py：生成器表达式
来源：http://hz.shanyushiyangtech.top/gtpnbsxgwf.html

(x * 2 for x in arr)
来源：http://hz.zhaomingkeji.xyz/gtsarssklg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zdqjudy.top/gtzsfepmmg.html

Counter(arr).most_common(3)
来源：http://hz.ehwqpu.com/gtjnpoftqn.html

[U13] Py：固定长度队列
来源：http://hz.cheryme.top/gtmctdpxeo.html

deque(maxlen=10)
来源：http://hz.yj202588.top/gtbirtlryz.html

[U14] Py：分组收集到列表
来源：http://hz.quarkkingdee.top/gtutjdvzie.html

defaultdict(list)
来源：http://hz.yonumen.top/gtbfpmwbwj.html

[U15] Py：高精度计时
来源：http://hz.gogol.net.cn/gtrphufloc.html

t = time.perf_counter()
来源：http://hz.sweek.top/gttmpbhnyp.html

[U16] Py：命令行参数解析
来源：http://hz.chenjidiqi.icu/gtghfqgvmk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cashguo.top/gtykhtsrvc.html

[U17] Py：初始化日志
来源：http://hz.dianchejie.cn/gtjwukpsrd.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shzxlz.cn/gtdgmahluq.html

[U18] Py：预编译正则
来源：http://hz.zhijiandao.cn/gtejdatlqo.html

pat = re.compile(r"\d+")
来源：http://hz.bjfxy.top/gtykoqvmyq.html

[U19] Py：正则替换带回调
来源：http://hz.andypj.xyz/gtnjjilkqx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.316326.xyz/gtncddthma.html

[U20] Py：缓存函数结果
来源：http://hz.ybcxt.top/gtqeuzmwgs.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhengqikj.top/gtbckgbqri.html

[U21] Py：自定义上下文管理器
来源：http://hz.chenlongwang.top/gtmxrpinfs.html

@contextlib.contextmanager
来源：http://hz.wangdashe.top/gtmiuiakyv.html

[U22] Py：矩阵转置
来源：http://hz.xziqi.cn/gtvsqhacku.html

list(zip(*m))
来源：http://hz.shzxlz.cn/gtzlrqvads.html

[U23] Py：分块读取大文件
来源：http://hz.feifeiyinyue.top/gtokxzjmrj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.guowangkeji.top/gtznctiveu.html

[U24] Py：路径操作
来源：http://hz.jlsjyb.cn/gtwmzatlio.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.fengsongda.top/gthxnkzfts.html

[U25] Py：CSV 按字典读
来源：http://hz.chenzaomai.com/gtifgrnqyj.html

csv.DictReader(f)
来源：http://hz.vqdsnc.cn/gtvkxthxcw.html

[U26] Py：并发下载
来源：http://hz.pycfn.com/gtcxkbvpqf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xuanzx.com/gtyoxcttoo.html

[U27] Py：异步 HTTP
来源：http://hz.mhx1999.top/gtovtnaltw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.dianchejie.cn/gtezrueqpl.html

[U28] Py：类型别名
来源：http://hz.sxryk.cn/gtjjmgwxqy.html

UserId = int
来源：http://hz.ywan-chungtsiang.top/gtqppcnsnq.html

[U29] Py：属性校验
来源：http://hz.tanke756.top/gtkmmgxkbb.html

@property 与 @x.setter 配合
来源：http://hz.yvedp.cn/gtyduiphxy.html

[U30] Py：数据类
来源：http://hz.jinqigufen.top/gtcrsecrnx.html

@dataclass(slots=True)
来源：http://hz.sufxvd.cn/gtvpjamjss.html

[U31] Py：单测
来源：http://hz.tianlin.xyz/gtpqjrffcp.html

python -m pytest -q
来源：http://hz.tian-w.cn/gtcuujmnri.html

[U32] Py：代码格式化
来源：http://hz.jinqigufen.top/gtygsjijmx.html

ruff format . && ruff check --fix .
来源：http://hz.yuanzhike.top/gtzjvuhiio.html

[U33] Py：打包发布
来源：http://hz.sweek.top/gtpbpweksj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yj202588.top/gtvbmvyucf.html

[U34] Py：判断编码
来源：http://hz.vqdsnc.cn/gtvruyxxlf.html

chardet.detect(raw)
来源：http://hz.haohaochexian.top/gtxmrgzouj.html

[U35] Py：发送邮件
来源：http://hz.yonumen.top/gtsgwdglah.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.meibo888.top/gtxderygte.html

[U36] Py：定时任务
来源：http://hz.haohaochexian.top/gtmdbcmpqa.html

schedule.every(10).minutes.do(job)
来源：http://hz.cashguo.top/gtdsgssqwf.html

[U37] Py：读写 Excel
来源：http://hz.pengpengdd.cyou/gtpmlpfhgb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yj20258.top/gtnznqajvh.html

[U38] Py：获取脚本所在目录
来源：http://hz.jinyuanbaomall.cn/gtcbkqeuqm.html

Path(__file__).resolve().parent
来源：http://hz.aizwys.cn/gtgqdrfzxk.html

[U39] Py：判断是否在交互环境
来源：http://hz.yangfankeji.com/gtohwxqzqz.html

sys.stdout.isatty()
来源：http://hz.yj20258888.top/gtpbxpkkbi.html

[U40] Py：打印到标准错误
来源：http://hz.c1oappe.top/gtplzracbn.html

print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gtqwcoxcvg.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cheryme.top/gtibluruno.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.52xcode.cn/gtltvfaien.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zycfv.cn/gttfdfywxd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.nwbrower.top/gtlismpbql.html

[U43] PHP：声明命名空间
来源：http://hz.xinyue.icu/gtjsewhclj.html

namespace App\Http;
来源：http://hz.pycfn.com/gtdthmmsvn.html

[U44] PHP：开启严格类型
来源：http://hz.quarkkingdee.top/gtpobuirja.html

declare(strict_types=1);
来源：http://hz.jianghu66.top/gtyzqwbclq.html

[U45] PHP：类型声明与返回类型
来源：http://hz.0kj1m.cn/gtizuaygun.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtgzpwcahy.html

[U46] PHP：可空类型
来源：http://hz.yanxiufei.cn/gtmxaxybhr.html

?string $name = null
来源：http://hz.gzhubu.top/gtoxyvxiky.html

[U47] PHP：联合类型
来源：http://hz.bjfxy.top/gtbktrbfvj.html

int|string $id
来源：http://hz.yueranfly.top/gtoqvfznod.html

[U48] PHP：纯枚举
来源：http://hz.haohaochexian.top/gtfwkoefrx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.chenzaomai.com/gtbutwxdle.html

[U49] PHP：只读属性
来源：http://hz.hongshengwenyu.top/gtcrumhghk.html

public readonly string $name
来源：http://hz.xinyue.icu/gtxkscvkfd.html

[U50] PHP：构造器属性提升
来源：http://hz.sysykeji.top/gtenyhbhwr.html

public function __construct(private int $id) {}
来源：http://hz.birdmap.top/gtqigtlpky.html

[U51] PHP：数组解构
来源：http://hz.shanyushiyangkeji.top/gtgrpudrxf.html

[$a, $b] = $arr;
来源：http://hz.zhiwuduotai.top/gtxtrsqdwt.html

[U52] PHP：箭头函数
来源：http://hz.feifeiyinyue.top/gtgqufnxya.html

$double = fn($x) => $x * 2;
来源：http://hz.snrcjt.cn/gtwsukrhcy.html

[U53] PHP：空合并运算符
来源：http://hz.zhiwuduotai.top/gtxbtshusb.html

$v = $a ?? $b ?? "default";
来源：http://hz.cheryme.top/gtvnjyhjqw.html

[U54] PHP：空安全调用
来源：http://hz.guowangkeji.top/gtvsyoemph.html

$obj?->method()
来源：http://hz.jqgufenzy.top/gtvsrtrfcl.html

[U55] PHP：match 表达式
来源：http://hz.chenzaomai.com/gtdogqltoe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj20258888.top/gtozerbmac.html

[U56] PHP：命名参数
来源：http://hz.sysykeji.top/gtryvywvkh.html

f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtneccuweb.html

[U57] PHP：字符串插值
来源：http://hz.gogol.net.cn/gtlqbsojcx.html

"值: {$a}"
来源：http://hz.jqgfzy.top/gtwqttqzcq.html

[U58] PHP：数组三件套
来源：http://hz.ydjk.org.cn/gtotiqlqig.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sufxvd.cn/gtjutxfnso.html

[U59] PHP：自定义排序
来源：http://hz.ybcxt.top/gtmvhjjgft.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cqqwz.cn/gtupbdogaf.html

[U60] PHP：JSON 编解码
来源：http://hz.hongshengwenyu.top/gtbcsjobxs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.dianchejie.cn/gtcwyjmuus.html

[U61] PHP：正则
来源：http://hz.shanyushiyangtech.top/gtqymvsgfd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtepshpwvt.html

[U62] PHP：日期对象
来源：http://hz.cheryme.top/gtqpwxzbll.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.xinyue.icu/gtsyxyeawb.html

[U63] PHP：文件读写
来源：http://hz.tanke756.top/gtxpmrylyp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.andypj.xyz/gtdormnwju.html

[U64] PHP：目录遍历
来源：http://hz.jqgfzy.top/gtipsehtek.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xuanzx.com/gtkfyjadce.html

[U65] PHP：会话
来源：http://hz.gaohongyu789.top/gtuofuhdko.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhiwuduotai.top/gtqejaosph.html

[U66] PHP：设置 Cookie
来源：http://hz.haohaochexian.top/gtipvpbnxj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinqigfzy.top/gttaqnfzhy.html

[U67] PHP：处理文件上传
来源：http://hz.wangshuangyany.cn/gtzdlcqfxk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.guannengcc.top/gtmoivdjdm.html

[U68] PHP：PDO 连接
来源：http://hz.c1oappe.top/gtncykpbde.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yonumen.top/gtegwrwyvf.html

[U69] PHP：PDO 预处理
来源：http://hz.gogol.net.cn/gtelyqqygg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hnxiangtu.top/gtxphpfsdg.html

[U70] PHP：PDO 事务
来源：http://hz.hfpthk.cn/gtxlobbcwe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.wangshuangyany.cn/gtnoejhcqb.html

[U71] PHP：抛出异常
来源：http://hz.hnxiangtu.top/gtfvhpirqr.html

throw new RuntimeException("失败", 500);
来源：http://hz.nwbrower.top/gtaejdkmnb.html

[U72] PHP：写错误日志
来源：http://hz.snrcjt.cn/gtegzzwrxc.html

error_log("失败: " . $e->getMessage());
来源：http://hz.c1oappe.top/gtkjbgclnq.html

[U73] PHP：读取 ini 配置
来源：http://hz.bjfxy.top/gttkwfesjs.html

parse_ini_file("config.ini", true)
来源：http://hz.xziqi.cn/gtjnrxjyel.html

[U74] PHP：读取环境变量
来源：http://hz.jqgufenzy.top/gtgfoxftlh.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shzxlz.cn/gtktlkoqhn.html

[U75] PHP：依赖注入
来源：http://hz.jqgufenzy.top/gtpdjyaojv.html

composer require psr/container
来源：http://hz.xuanzx.com/gtgjrsxhcj.html

[U76] PHP：简单路由
来源：http://hz.fzhhl.top/gtjkpnqtej.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jianghu66.top/gtazutmwyj.html

[U77] PHP：模板渲染
来源：http://hz.fzhhl.top/gtjchoejjw.html

composer require twig/twig
来源：http://hz.jinqigufen.top/gtyhspyugq.html

[U78] PHP：单元测试
来源：http://hz.fengsongda.top/gtgdwlekeg.html

composer require --dev phpunit/phpunit
来源：http://hz.yuxming.cn/gtsdcezbdr.html


<!-- 参考信息 -->