代发 wailian999

int size() const noexcept { return n_; }
来源：http://hz.andypj.xyz/gtsywvfirm.html

[S53] C++：移动语义
来源：http://hz.sxryk.cn/gtxlcppelv.html

std::vector<int> w = std::move(v);
来源：http://hz.gzhubu.top/gtzszyjpoh.html

[S54] C++：异常处理
来源：http://hz.yanxiufei.cn/gtwudvwgqo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxuanxn.top/gttttqgvon.html

[S55] C++：结构化绑定
来源：http://hz.hammf.cn/gtqugkqpjc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gaohongyu789.top/gtzzdgdehb.html

[S56] C++：optional
来源：http://hz.jinqigfzy.top/gtcfczhrjm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnqzz.top/gtcsqnzajm.html

[S57] C++：编译期常量
来源：http://hz.fzhhl.top/gtxkoabrqp.html

constexpr int N = 10;
来源：http://hz.yanxiufei.cn/gtszuinahh.html

[S58] C++：命名空间
来源：http://hz.hysaishi.cn/gthbvtdyor.html

namespace ns { int f() { return 1; } }
来源：http://hz.cdnleiting.top/gtvdnsavxc.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gtiknqblfc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xuanzx.com/gtyfhklccb.html

[S60] C++：遍历并删除元素
来源：http://hz.jlsjyb.cn/gtuwqjtxvn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtrmthebpw.html

================================================================================
来源：http://hz.nanxuanxn.top/gtktoflcqa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.redwolf501.top/gtejbwrpdh.html

================================================================================
来源：http://hz.9152youxi.cn/gtdqkayycf.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangkeji.top/gteuzieiii.html

println("Hello")
来源：http://hz.hfpthk.cn/gtlyjzblhj.html

[T02] Kotlin：变量
来源：http://hz.jianghu66.top/gtdivvxeec.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yonumen.top/gtanswcrcd.html

[T03] Kotlin：字符串模板
来源：http://hz.cdnleiting.top/gtmzcpbrgs.html

"值: $b"
来源：http://hz.fengsongda.top/gtpnjyszgb.html

[T04] Kotlin：空安全
来源：http://hz.cdnleiting.top/gtuerqyyna.html

val n: String? = null;  n?.length
来源：http://hz.shzxlz.cn/gttvhnauuo.html

[T05] Kotlin：when 表达式
来源：http://hz.cashguo.top/gtrburibkc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gogol.net.cn/gtsrrqhpnv.html

[T06] Kotlin：集合映射
来源：http://hz.wangshuangyany.cn/gtwakohtpx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.fengsongda.top/gtypsduhnw.html

[T07] Kotlin：集合过滤
来源：http://hz.gotoacloud.top/gtkyfherqs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hysaishi.cn/gtqejdusks.html

[T08] Kotlin：数据类
来源：http://hz.birdmap.top/gtampmnunm.html

data class User(val name: String, val age: Int)
来源：http://hz.snrcjt.cn/gtikmbyjbk.html

[T09] Kotlin：扩展函数
来源：http://hz.yongpay.top/gtnakegblq.html

fun String.exclaim() = this + "!"
来源：http://hz.52xcode.cn/gtwwntustr.html

[T10] Kotlin：默认参数
来源：http://hz.bjfxy.top/gtsevlwvqg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.guannengcc.top/gtoymtaclx.html

[T11] Kotlin：协程
来源：http://hz.pycfn.com/gtaeqwmche.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daria6918.cn/gtprloxklz.html

[T12] Kotlin：解构声明
来源：http://hz.yj202588.top/gteqryhaxt.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydjk.org.cn/gtztofqmne.html

[T13] Kotlin：只读 Map
来源：http://hz.kuanghao11.cn/gtrpottnfo.html

val m = mapOf("a" to 1)
来源：http://hz.yongpay.top/gthesvvzhf.html

[T14] Kotlin：循环
来源：http://hz.haohaochexian.top/gtgoqjkpfr.html

for (i in 1..10) println(i)
来源：http://hz.birdmap.top/gtbvnpuhfd.html

[T15] Kotlin：接口
来源：http://hz.iojbl.cn/gtzvudxrpl.html

interface Shape { fun area(): Double }
来源：http://hz.hywenlv.cn/gtpnntgczw.html

[T16] Swift：Hello World
来源：http://hz.zhijiandao.cn/gtjtlyscis.html

print("Hello")
来源：http://hz.gogol.net.cn/gttcgdewrj.html

[T17] Swift：变量与常量
来源：http://hz.mhx1999.top/gtncnxuhwl.html

var a = 1;  let b = 2
来源：http://hz.yanxiufei.cn/gtxzfuiypb.html

[T18] Swift：字符串插值
来源：http://hz.jinqigfzy.top/gtvxwabkso.html

"值: \(b)"
来源：http://hz.chenlongwang.top/gtsmicnwyn.html

[T19] Swift：可选绑定
来源：http://hz.dianchejie.cn/gtuytkrbwr.html

if let n = opt { print(n) }
来源：http://hz.xinyue.icu/gteutxrupu.html

[T20] Swift：数组操作
来源：http://hz.andypj.xyz/gthmqjicnc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ydjk.org.cn/gtzmdklnyj.html

[T21] Swift：遍历
来源：http://hz.yangfankeji.com/gtcgxwygbl.html

for x in a { print(x) }
来源：http://hz.xziqi.cn/gtnkmwutvu.html

[T22] Swift：字典
来源：http://hz.shuidangran.top/gtlzysggxh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zycfv.cn/gtjdewwagc.html

[T23] Swift：函数
来源：http://hz.tanke756.top/gtkkiauydr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hammf.cn/gtdbagktih.html

[T24] Swift：闭包
来源：http://hz.jqgfzy.top/gtlnptidbi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuxming.cn/gtdcoanjdv.html

[T25] Swift：结构体
来源：http://hz.yangfankeji.com/gtiuljywon.html

struct P { var x: Int }
来源：http://hz.ivvv.top/gtztdcdkna.html

[T26] Swift：类与重写
来源：http://hz.dashuyun.cn/gtsvewmxni.html

class A: Base { override func f() {} }
来源：http://hz.xingfuxueyuan.xyz/gtasdkmxtd.html

[T27] Swift：错误处理
来源：http://hz.hnxiangtu.top/gtecuaithx.html

do { try f() } catch { print(error) }
来源：http://hz.birdmap.top/gtwautufyn.html

[T28] Swift：枚举
来源：http://hz.shzxlz.cn/gtoqsvbjkf.html

enum Color { case red, green }
来源：http://hz.sysykeji.top/gtsqpimiac.html

[T29] Swift：guard 提前返回
来源：http://hz.jianghu66.top/gtaswrnqad.html

guard let x = opt else { return }
来源：http://hz.mhx1999.top/gthudjwnew.html

[T30] Swift：协议
来源：http://hz.gotoacloud.top/gtnrudslbp.html

protocol Shape { func area() -> Double }
来源：http://hz.zhoulong.xyz/gttaegitwk.html

[T31] Lua：Hello World
来源：http://hz.dashuyun.cn/gtbqjiatgu.html

print("Hello")
来源：http://hz.snrcjt.cn/gtgknqqbjs.html

[T32] Lua：局部变量
来源：http://hz.wangdashe.top/gtpsifprtc.html

local a = 1
来源：http://hz.cucudq.cn/gtqhuquejc.html

[T33] Lua：表（数组）
来源：http://hz.quarkkingdee.top/gtssbtdmig.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yueranfly.top/gtgpdoxbmf.html

[T34] Lua：遍历表
来源：http://hz.316326.xyz/gtvlzuwllu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.andypj.xyz/gtmjbwhnsj.html

[T35] Lua：字典表
来源：http://hz.yonumen.top/gtdvbklgin.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ydzc1.top/gtyvcpurwy.html

[T36] Lua：函数
来源：http://hz.yonumen.top/gtvdjrorpw.html

function add(a, b) return a + b end
来源：http://hz.xinyue.icu/gtmzqncsdv.html

[T37] Lua：字符串拼接
来源：http://hz.wangshuangyany.cn/gtyenzokgn.html

"a" .. "b"
来源：http://hz.yanxiufei.cn/gtnlsjgmrs.html

[T38] Lua：条件
来源：http://hz.redwolf501.top/gtusgivpfw.html

if x > 0 then print("正") end
来源：http://hz.cheryme.top/gtwxwlgexo.html

[T39] Lua：模式匹配
来源：http://hz.jqgfzy.top/gtpxqhhzqf.html

string.find(s, "%d+")
来源：http://hz.zhixingplan.top/gtehoaexoi.html

[T40] Lua：元表
来源：http://hz.ydzc1.top/gtsvpganzm.html

setmetatable({}, { __index = base })
来源：http://hz.9152youxi.cn/gtupdqhwjw.html

[T41] Perl：Hello World
来源：http://hz.andypj.xyz/gtkjewhlsm.html

print "Hello\n";
来源：http://hz.tanke756.top/gttdrgocam.html

[T42] Perl：变量类型
来源：http://hz.wangshuangyany.cn/gtelczldnz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cqqwz.cn/gtdmbwoptn.html

[T43] Perl：字符串插值
来源：http://hz.316326.xyz/gtiunuwoym.html

"值: $a"
来源：http://hz.zycfv.cn/gtdhityrqh.html

[T44] Perl：条件
来源：http://hz.xinyue.icu/gtafezjkzc.html

if ($a > 0) { print "正"; }
来源：http://hz.yanxiufei.cn/gtlqltdfvg.html

[T45] Perl：数组遍历
来源：http://hz.zhixingplan.top/gtdkqwysdt.html

for my $x (@arr) { print $x; }
来源：http://hz.shangyingyoupin.top/gtqldaguxa.html

[T46] Perl：哈希操作
来源：http://hz.zycfv.cn/gttrnxsvjf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cashguo.top/gtaumhmihu.html

[T47] Perl：正则捕获
来源：http://hz.tian-w.cn/gtgxpcnpik.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cqqwz.cn/gtjxobfpto.html

[T48] Perl：正则替换
来源：http://hz.fzhhl.top/gteqmbrcpq.html

$s =~ s/old/new/g;
来源：http://hz.sysykeji.top/gtfaxxinfv.html

[T49] Perl：函数
来源：http://hz.bjfxy.top/gtubpoxoql.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gzhubu.top/gtfydaqqyz.html

[T50] Perl：逐行读文件
来源：http://hz.mhx1999.top/gtwwcfsyin.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cqqwz.cn/gtmxzxfvyo.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xylfe.cn/gtzxovglbu.html

[T51] Scala：Hello World
来源：http://hz.ybcxt.top/gtfjvwmnwf.html

println("Hello")
来源：http://hz.yuanzhike.top/gtwmyqzscx.html

[T52] Scala：变量
来源：http://hz.zhengqikj.top/gtocykstdk.html

val a = 1;  var b = 2
来源：http://hz.zhixingplan.top/gtfvwbspyg.html

[T53] Scala：字符串插值
来源：http://hz.bjfxy.top/gtckwxpqdc.html

s"值: $b"
来源：http://hz.daxiang520.top/gtiwutbhtr.html

[T54] Scala：集合映射
来源：http://hz.sysykeji.top/gttlnivoux.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.0kj1m.cn/gtpjhvuaan.html

[T55] Scala：集合过滤
来源：http://hz.hywenlv.cn/gtpwbakoae.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinqigufen.top/gtvyhotyse.html

[T56] Scala：样例类
来源：http://hz.cqqwz.cn/gtnhhvnygi.html

case class User(name: String, age: Int)
来源：http://hz.tanke756.top/gttssciyjt.html

[T57] Scala：模式匹配
来源：http://hz.yongpay.top/gtqrilpcxv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nanxuanxn.top/gtfbrtpxqx.html

[T58] Scala：函数定义
来源：http://hz.meibo888.top/gtvhdfohiv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenlongwang.top/gtxvvgkzwy.html

[T59] Scala：循环
来源：http://hz.iojbl.cn/gtijsdroxg.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhijiandao.cn/gtojsydkjl.html

[T60] Scala：折叠
来源：http://hz.ywan-chungtsiang.top/gtpwenvcfv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.smart0.xyz/gtxelpuihe.html

================================================================================
来源：http://hz.zhixingplan.top/gtdqhsufer.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhixingplan.top/gteyzigzmf.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmufgampw.html

[U01] Py：创建虚拟环境
来源：http://hz.ivvv.top/gtiamittyl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hongshengwenyu.top/gtzttvkfhw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fengsongda.top/gtkfdkxpdt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.9152youxi.cn/gtzhsgnvjo.html

[U03] Py：加载 .env 配置
来源：http://hz.shanyushiyangkeji.top/gtjsljgfum.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhixingplan.top/gtpbtgcbjr.html

[U04] Py：变量调试打印
来源：http://hz.havefunace.top/gtqwqgbxyt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jyoumei.cn/gtyiofswji.html

[U05] Py：列表去重且保序
来源：http://hz.zhengqikj.top/gtfvstmpes.html

list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangtech.top/gtgbeloekl.html

[U06] Py：合并两个字典
来源：http://hz.jianghu66.top/gtszdjaxmx.html

{**a, **b}
来源：http://hz.tanke756.top/gtbxjgytac.html

[U07] Py：反转字典键值
来源：http://hz.jinqigufen.top/gtqkhyjnom.html

{v: k for k, v in d.items()}
来源：http://hz.snrcjt.cn/gtrnasdpsx.html

[U08] Py：展平二维列表
来源：http://hz.ppjwa.cn/gtintyqfkl.html

[y for x in nested for y in x]
来源：http://hz.pengpengdd.cyou/gtwcxktbtw.html

[U09] Py：字典取最大值的键
来源：http://hz.shanyushiyangkeji.top/gtcihajnby.html

max(d, key=d.get)
来源：http://hz.bjfxy.top/gtlfafzpuz.html

[U10] Py：按值排序字典
来源：http://hz.svipenyu.cn/gtboauxxfq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hnqzz.top/gtxvjoditd.html

[U11] Py：生成器表达式
来源：http://hz.ppjwa.cn/gtiahyoahe.html

(x * 2 for x in arr)
来源：http://hz.ppjwa.cn/gtembzuoyb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.sysykeji.top/gtzkxqtzcu.html

Counter(arr).most_common(3)
来源：http://hz.pycfn.com/gtydxvugqe.html

[U13] Py：固定长度队列
来源：http://hz.yangfankeji.com/gtbqsoofyx.html

deque(maxlen=10)
来源：http://hz.yanxiufei.cn/gtxjwfydzi.html

[U14] Py：分组收集到列表
来源：http://hz.nanxinkj.top/gtsbkfcbjv.html

defaultdict(list)
来源：http://hz.jinqigufen.top/gtpfqwybgz.html

[U15] Py：高精度计时
来源：http://hz.pengpengdd.cyou/gtbbpkwrno.html

t = time.perf_counter()
来源：http://hz.hnxiangtu.top/gtnzzpldxy.html

[U16] Py：命令行参数解析
来源：http://hz.9152youxi.cn/gtebbqthpu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ehwqpu.com/gtwucjeayz.html

[U17] Py：初始化日志
来源：http://hz.zhoulong.xyz/gtommyqali.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shuidangran.top/gtznrnieoo.html

[U18] Py：预编译正则
来源：http://hz.zdqjudy.top/gtrsravzfs.html

pat = re.compile(r"\d+")
来源：http://hz.hammf.cn/gtdcaqttcw.html

[U19] Py：正则替换带回调
来源：http://hz.birdmap.top/gtaejzlnzf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jqgfzy.top/gtwtmaaggf.html

[U20] Py：缓存函数结果
来源：http://hz.sxryk.cn/gtdlnxukkp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.daxiang520.top/gtuwdhorss.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhixingplan.top/gtjqxdgizf.html

@contextlib.contextmanager
来源：http://hz.yj202588.top/gtyispoogh.html

[U22] Py：矩阵转置
来源：http://hz.0kj1m.cn/gttnjfdrrn.html

list(zip(*m))
来源：http://hz.yj20258.top/gtvdzgymyo.html

[U23] Py：分块读取大文件
来源：http://hz.jianghu66.top/gtmreflzec.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cheryme.top/gtvqbbgzxz.html

[U24] Py：路径操作
来源：http://hz.yuxming.cn/gtmwhocbdv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hammf.cn/gtngyuawgx.html

[U25] Py：CSV 按字典读
来源：http://hz.cqqwz.cn/gtwtisfvbu.html

csv.DictReader(f)
来源：http://hz.sxryk.cn/gtlpncdaqs.html

[U26] Py：并发下载
来源：http://hz.jqgfzy.top/gtncqhorsu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jiagoushi.top/gtvwlcyase.html

[U27] Py：异步 HTTP
来源：http://hz.yangfankeji.com/gthbhycxbs.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hnxiangtu.top/gtqoogmzcg.html

[U28] Py：类型别名
来源：http://hz.gogol.net.cn/gtqnnlsvrv.html

UserId = int
来源：http://hz.yuanzhike.top/gtcgbymafe.html

[U29] Py：属性校验
来源：http://hz.zhengqikj.top/gthbvrsptu.html

@property 与 @x.setter 配合
来源：http://hz.zdqjudy.top/gtdmwydkgj.html

[U30] Py：数据类
来源：http://hz.shanyushiyangtech.top/gtwpuqkjsu.html

@dataclass(slots=True)
来源：http://hz.hywenlv.cn/gtlzkrqxoy.html

[U31] Py：单测
来源：http://hz.nwbrower.top/gtyodhgcbw.html

python -m pytest -q
来源：http://hz.nwbrower.top/gtszdbmkkt.html

[U32] Py：代码格式化
来源：http://hz.shzxlz.cn/gtovpdguss.html

ruff format . && ruff check --fix .
来源：http://hz.jqgfzy.top/gtinujyopp.html

[U33] Py：打包发布
来源：http://hz.xingfuxueyuan.xyz/gtobshfnjz.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.iojbl.cn/gtesomtues.html

[U34] Py：判断编码
来源：http://hz.dianchejie.cn/gtzzppblqj.html

chardet.detect(raw)
来源：http://hz.sysykeji.top/gtbyrwgysd.html

[U35] Py：发送邮件
来源：http://hz.cashguo.top/gtxauevpky.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jinghuilouyu.cn/gtsktiiujl.html

[U36] Py：定时任务
来源：http://hz.yangfankeji.com/gtlrljksoi.html

schedule.every(10).minutes.do(job)
来源：http://hz.9152youxi.cn/gtxgyiscfj.html

[U37] Py：读写 Excel
来源：http://hz.daria6918.cn/gtnnnjxbdz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yonumen.top/gtzziktqrw.html

[U38] Py：获取脚本所在目录
来源：http://hz.wangshuangyany.cn/gtaiqoydgc.html

Path(__file__).resolve().parent
来源：http://hz.yj20258.top/gtexssdvna.html

[U39] Py：判断是否在交互环境
来源：http://hz.vqdsnc.cn/gtoliuraga.html

sys.stdout.isatty()
来源：http://hz.bjfxy.top/gtxhjajfvt.html

[U40] Py：打印到标准错误
来源：http://hz.ivvv.top/gtmuwegoii.html

print("err", file=sys.stderr)
来源：http://hz.zhongyouzk.top/gtgrcavjwc.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.52xcode.cn/gtqdgkspzv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.0kj1m.cn/gtniaxkprm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.iojbl.cn/gtzkeynjfc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.316326.xyz/gtdtizlxjo.html

[U43] PHP：声明命名空间
来源：http://hz.chenlongwang.top/gtfnlkeepl.html

namespace App\Http;
来源：http://hz.52xcode.cn/gtjryzfntk.html

[U44] PHP：开启严格类型
来源：http://hz.shangyingyoupin.top/gtgovmnznx.html

declare(strict_types=1);
来源：http://hz.ywan-chungtsiang.top/gtuyrklvnu.html

[U45] PHP：类型声明与返回类型
来源：http://hz.iojbl.cn/gtasxafnkd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gtfonrzqht.html

[U46] PHP：可空类型
来源：http://hz.sxryk.cn/gtynxbtdqx.html

?string $name = null
来源：http://hz.xuanzx.com/gtlygiriuv.html

[U47] PHP：联合类型
来源：http://hz.xingfuxueyuan.xyz/gtniwijxfv.html

int|string $id
来源：http://hz.zhixingplan.top/gtnjklxlzt.html

[U48] PHP：纯枚举
来源：http://hz.yvedp.cn/gtzvrvoixn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yuxming.cn/gtqsycllqm.html

[U49] PHP：只读属性
来源：http://hz.0kj1m.cn/gtttmmlnqd.html

public readonly string $name
来源：http://hz.shanyushiyangkeji.top/gtwkeepweb.html

[U50] PHP：构造器属性提升
来源：http://hz.zycfv.cn/gteqaaaewf.html

public function __construct(private int $id) {}
来源：http://hz.jiagoushi.top/gtildenbjh.html

[U51] PHP：数组解构
来源：http://hz.zhongyouzk.top/gtckpaecwa.html

[$a, $b] = $arr;
来源：http://hz.nanxuanxn.top/gtheekclyt.html

[U52] PHP：箭头函数
来源：http://hz.gotoacloud.top/gtfpfzxhsr.html

$double = fn($x) => $x * 2;
来源：http://hz.sxryk.cn/gtdwmyshxq.html

[U53] PHP：空合并运算符
来源：http://hz.jiagoushi.top/gtzweterij.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhiwuduotai.top/gtvbpeakin.html

[U54] PHP：空安全调用
来源：http://hz.meibo888.top/gtbxiwetqe.html

$obj?->method()
来源：http://hz.ywan-chungtsiang.top/gtantccstw.html

[U55] PHP：match 表达式
来源：http://hz.quarkkingdee.top/gtkwkemxsj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jyoumei.cn/gtqrmgmgwl.html

[U56] PHP：命名参数
来源：http://hz.dashuyun.cn/gtetsqwwwa.html

f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtavnamcdh.html

[U57] PHP：字符串插值
来源：http://hz.iojbl.cn/gtchmvkuho.html

"值: {$a}"
来源：http://hz.zdqjudy.top/gtjwvlturm.html

[U58] PHP：数组三件套
来源：http://hz.yonumen.top/gttdidgcnv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ydjk.org.cn/gtilxgveyr.html

[U59] PHP：自定义排序
来源：http://hz.jqgufenzy.top/gtxvxosbce.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guowangkeji.top/gtrqjjprie.html

[U60] PHP：JSON 编解码
来源：http://hz.jinqigfzy.top/gtjcvmrbui.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.quarkkingdee.top/gtglajczaa.html

[U61] PHP：正则
来源：http://hz.xuetiantiany.cn/gtoaouzqhe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.c1oappe.top/gtrxnksfyj.html

[U62] PHP：日期对象
来源：http://hz.jqgufenzy.top/gtdwqdbwae.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhijiandao.cn/gtdetiurej.html

[U63] PHP：文件读写
来源：http://hz.xylfe.cn/gtipajvhpv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj20258888.top/gtkuaggikw.html

[U64] PHP：目录遍历
来源：http://hz.jinqigufen.top/gtahuxntct.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hongshengwenyu.top/gtiuukdhlo.html

[U65] PHP：会话
来源：http://hz.havefunace.top/gtyzrunglf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.chenjidiqi.icu/gtnffzsieq.html

[U66] PHP：设置 Cookie
来源：http://hz.yangfankeji.com/gtdiwbasjz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xuetiantiany.cn/gtllqjfrjq.html

[U67] PHP：处理文件上传
来源：http://hz.svipenyu.cn/gtpvoxeixd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yj20258.top/gtdfhsstsb.html

[U68] PHP：PDO 连接
来源：http://hz.cdnleiting.top/gtvvzqellk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.tanke756.top/gtogcffhiu.html

[U69] PHP：PDO 预处理
来源：http://hz.xuetiantiany.cn/gtlwiweucl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.svipenyu.cn/gthmvwgecc.html

[U70] PHP：PDO 事务
来源：http://hz.iojbl.cn/gteondugar.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.daxiang520.top/gtgqjimucj.html

[U71] PHP：抛出异常
来源：http://hz.yj202588.top/gtiztnstju.html

throw new RuntimeException("失败", 500);
来源：http://hz.quarkkingdee.top/gtjugjjivh.html

[U72] PHP：写错误日志
来源：http://hz.yonumen.top/gtkuppygre.html

error_log("失败: " . $e->getMessage());
来源：http://hz.chenlongwang.top/gtstczewhm.html

[U73] PHP：读取 ini 配置
来源：http://hz.zdqjudy.top/gtikbrfuxb.html

parse_ini_file("config.ini", true)
来源：http://hz.haohaochexian.top/gtwviyjfoy.html

[U74] PHP：读取环境变量
来源：http://hz.chenzaomai.com/gtejbulhah.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gaohongyu789.top/gtcqfsidtw.html

[U75] PHP：依赖注入
来源：http://hz.zhiwuduotai.top/gtcsqjvelh.html

composer require psr/container
来源：http://hz.smart0.xyz/gtwpkedzss.html

[U76] PHP：简单路由
来源：http://hz.gzhubu.top/gtegadsnef.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zycfv.cn/gtrlwhkbjn.html

[U77] PHP：模板渲染
来源：http://hz.xylfe.cn/gtrodjohon.html

composer require twig/twig
来源：http://hz.aibaodan.cn/gtilmugaji.html

[U78] PHP：单元测试
来源：http://hz.bjfxy.top/gtwhhtcgek.html

composer require --dev phpunit/phpunit
来源：http://hz.zhiwuduotai.top/gtthtdvmpq.html


<!-- 参考信息 -->