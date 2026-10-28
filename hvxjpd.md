代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.svipenyu.cn/gtjypckiri.html

[S55] C++：结构化绑定
来源：http://hz.cqqwz.cn/gthxhbkqtk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nanxinkj.top/gtivsmrkae.html

[S56] C++：optional
来源：http://hz.yj202588.top/gtixwmujrj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hfpthk.cn/gtspowoiem.html

[S57] C++：编译期常量
来源：http://hz.daxiang520.top/gthzazersg.html

constexpr int N = 10;
来源：http://hz.nwbrower.top/gtfgghrrvi.html

[S58] C++：命名空间
来源：http://hz.yuanzhike.top/gtjahyzhbh.html

namespace ns { int f() { return 1; } }
来源：http://hz.52xcode.cn/gtndokocqm.html

[S59] C++：静态断言
来源：http://hz.dashuyun.cn/gtnvadauxg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cdnleiting.top/gtqnianvwj.html

[S60] C++：遍历并删除元素
来源：http://hz.dianchejie.cn/gtfyyyyxfc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhengqikj.top/gtrplnjxns.html

================================================================================
来源：http://hz.gogol.net.cn/gttklngpil.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenzaomai.com/gtxmlkkyar.html

================================================================================
来源：http://hz.zycfv.cn/gtdaplpgmh.html

[T01] Kotlin：Hello World
来源：http://hz.hnqzz.top/gtxxnzunna.html

println("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtttvwpqpn.html

[T02] Kotlin：变量
来源：http://hz.zhiwuduotai.top/gtnaftqrjb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hnqzz.top/gtammcmilo.html

[T03] Kotlin：字符串模板
来源：http://hz.tianlin.xyz/gtsigodzem.html

"值: $b"
来源：http://hz.zhiwuduotai.top/gthoyivkic.html

[T04] Kotlin：空安全
来源：http://hz.wangshuangyany.cn/gtbaysguax.html

val n: String? = null;  n?.length
来源：http://hz.snrcjt.cn/gttijrgbgo.html

[T05] Kotlin：when 表达式
来源：http://hz.jiagoushi.top/gtzhwthvxw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuanzhike.top/gtnzdogfps.html

[T06] Kotlin：集合映射
来源：http://hz.hnxiangtu.top/gtlhfgdsbw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.daxiang520.top/gttehshuri.html

[T07] Kotlin：集合过滤
来源：http://hz.dianchejie.cn/gtsirfdfla.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.smart0.xyz/gtvyxvicvy.html

[T08] Kotlin：数据类
来源：http://hz.fzhhl.top/gtolmlkyoc.html

data class User(val name: String, val age: Int)
来源：http://hz.chenjidiqi.icu/gtwvgrhhty.html

[T09] Kotlin：扩展函数
来源：http://hz.yanxiufei.cn/gteesryefr.html

fun String.exclaim() = this + "!"
来源：http://hz.yvedp.cn/gtlblsqlrz.html

[T10] Kotlin：默认参数
来源：http://hz.redwolf501.top/gtmrzpsrjb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.kuanghao11.cn/gtxbxiesde.html

[T11] Kotlin：协程
来源：http://hz.0kj1m.cn/gtdsrslugd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.wangshuangyany.cn/gtdhzjodff.html

[T12] Kotlin：解构声明
来源：http://hz.ybcxt.top/gtqvzlgvgr.html

val (a, b) = Pair(1, 2)
来源：http://hz.cqqwz.cn/gtnyfntsbc.html

[T13] Kotlin：只读 Map
来源：http://hz.zycfv.cn/gtpmukxjou.html

val m = mapOf("a" to 1)
来源：http://hz.zhongyouzk.top/gtbfehogtl.html

[T14] Kotlin：循环
来源：http://hz.kuanghao11.cn/gttfhkawhc.html

for (i in 1..10) println(i)
来源：http://hz.xylfe.cn/gtpinlutrx.html

[T15] Kotlin：接口
来源：http://hz.kuanghao11.cn/gtghbzqbyj.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258888.top/gtvgfanbtf.html

[T16] Swift：Hello World
来源：http://hz.ivvv.top/gtmtsahnlj.html

print("Hello")
来源：http://hz.wangshuangyany.cn/gtzfcgzaul.html

[T17] Swift：变量与常量
来源：http://hz.shanyushiyangkeji.top/gtqkppwfhl.html

var a = 1;  let b = 2
来源：http://hz.jinqigfzy.top/gteqthboqb.html

[T18] Swift：字符串插值
来源：http://hz.zhiwuduotai.top/gttogsyyrw.html

"值: \(b)"
来源：http://hz.chenzaomai.com/gtvmhftazq.html

[T19] Swift：可选绑定
来源：http://hz.jqgfzy.top/gtbvqeaubd.html

if let n = opt { print(n) }
来源：http://hz.zhiwuduotai.top/gtmuiddofw.html

[T20] Swift：数组操作
来源：http://hz.zhixingplan.top/gtbdzkarpl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sweek.top/gtaijiwcrf.html

[T21] Swift：遍历
来源：http://hz.iojbl.cn/gthtobdqud.html

for x in a { print(x) }
来源：http://hz.chenjidiqi.icu/gtrajecpud.html

[T22] Swift：字典
来源：http://hz.cqqwz.cn/gtdkrhgngx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.feifeiyinyue.top/gtujnpftnw.html

[T23] Swift：函数
来源：http://hz.jinqigfzy.top/gttvfffiyr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yj20258888.top/gtusajunov.html

[T24] Swift：闭包
来源：http://hz.gotoacloud.top/gtddieqqmy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.aizwys.cn/gtvfnpncra.html

[T25] Swift：结构体
来源：http://hz.snrcjt.cn/gtrzwgpdul.html

struct P { var x: Int }
来源：http://hz.zhixingplan.top/gthzugzife.html

[T26] Swift：类与重写
来源：http://hz.hnxiangtu.top/gtrbmirsdj.html

class A: Base { override func f() {} }
来源：http://hz.hysaishi.cn/gtkxenmldi.html

[T27] Swift：错误处理
来源：http://hz.316326.xyz/gtjqxrmzkf.html

do { try f() } catch { print(error) }
来源：http://hz.shanyushiyangtech.top/gtsbpkcrgq.html

[T28] Swift：枚举
来源：http://hz.yanxiufei.cn/gtdyymqcig.html

enum Color { case red, green }
来源：http://hz.daria6918.cn/gtxiabdkde.html

[T29] Swift：guard 提前返回
来源：http://hz.hongshengwenyu.top/gtbnhancty.html

guard let x = opt else { return }
来源：http://hz.iojbl.cn/gtyuhyhusa.html

[T30] Swift：协议
来源：http://hz.snrcjt.cn/gtnsnybvfv.html

protocol Shape { func area() -> Double }
来源：http://hz.hnxiangtu.top/gtbjpkovks.html

[T31] Lua：Hello World
来源：http://hz.feifeiyinyue.top/gtqgextiur.html

print("Hello")
来源：http://hz.ydzc1.top/gtnxmovjyz.html

[T32] Lua：局部变量
来源：http://hz.hnxiangtu.top/gtvjyomsqg.html

local a = 1
来源：http://hz.yangfankeji.com/gtnhudwbub.html

[T33] Lua：表（数组）
来源：http://hz.snrcjt.cn/gtnxskzvvf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.mhx1999.top/gtxtqkuisu.html

[T34] Lua：遍历表
来源：http://hz.zhengqikj.top/gtfmaljlfg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangshuangyany.cn/gtidfwzbmq.html

[T35] Lua：字典表
来源：http://hz.jianghu66.top/gtcyidbkmx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.nwbrower.top/gtlbbjjsjz.html

[T36] Lua：函数
来源：http://hz.xingfuxueyuan.xyz/gtohnxjxar.html

function add(a, b) return a + b end
来源：http://hz.hongshengwenyu.top/gtvqczmbst.html

[T37] Lua：字符串拼接
来源：http://hz.xuetiantiany.cn/gtijmjhhpg.html

"a" .. "b"
来源：http://hz.jinghuilouyu.cn/gtiqmfooym.html

[T38] Lua：条件
来源：http://hz.havefunace.top/gtkpzyzjhx.html

if x > 0 then print("正") end
来源：http://hz.tianlin.xyz/gtsmeuerqd.html

[T39] Lua：模式匹配
来源：http://hz.vqdsnc.cn/gtkbalbzhb.html

string.find(s, "%d+")
来源：http://hz.quarkkingdee.top/gtexaedlmc.html

[T40] Lua：元表
来源：http://hz.yangfankeji.com/gthbuikwlq.html

setmetatable({}, { __index = base })
来源：http://hz.havefunace.top/gtnzldxqkp.html

[T41] Perl：Hello World
来源：http://hz.daxiang520.top/gtshvjetjf.html

print "Hello\n";
来源：http://hz.dashuyun.cn/gtwhgkctdq.html

[T42] Perl：变量类型
来源：http://hz.cashguo.top/gttohfchwl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cqqwz.cn/gtzdgahpzt.html

[T43] Perl：字符串插值
来源：http://hz.ydjk.org.cn/gtfgjtxgax.html

"值: $a"
来源：http://hz.tian-w.cn/gtfbnoenhs.html

[T44] Perl：条件
来源：http://hz.yongpay.top/gtkujtqtbv.html

if ($a > 0) { print "正"; }
来源：http://hz.yangfankeji.com/gtkxhgtpml.html

[T45] Perl：数组遍历
来源：http://hz.9152youxi.cn/gtbjophres.html

for my $x (@arr) { print $x; }
来源：http://hz.daxiang520.top/gtnixayqtd.html

[T46] Perl：哈希操作
来源：http://hz.yangfankeji.com/gtchuzkfiy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ehwqpu.com/gttrlbeijc.html

[T47] Perl：正则捕获
来源：http://hz.yuanzhike.top/gtkfanzfqq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cqqwz.cn/gtaiafuygs.html

[T48] Perl：正则替换
来源：http://hz.jianghu66.top/gtvtrticbj.html

$s =~ s/old/new/g;
来源：http://hz.tianlin.xyz/gtenwuvitj.html

[T49] Perl：函数
来源：http://hz.zhoulong.xyz/gtgppueulv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtejowwbic.html

[T50] Perl：逐行读文件
来源：http://hz.quarkkingdee.top/gtfdqpkjom.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.redwolf501.top/gtwgszjkho.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yuanzhike.top/gtwrpcukmg.html

[T51] Scala：Hello World
来源：http://hz.aibaodan.cn/gtdfvfhbgd.html

println("Hello")
来源：http://hz.xinyue.icu/gtocuipdpo.html

[T52] Scala：变量
来源：http://hz.9152youxi.cn/gtrcjulaal.html

val a = 1;  var b = 2
来源：http://hz.yonumen.top/gtuiuclsjc.html

[T53] Scala：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtflkwnsxy.html

s"值: $b"
来源：http://hz.feifeiyinyue.top/gtcvftsndf.html

[T54] Scala：集合映射
来源：http://hz.xinyue.icu/gtxacclwur.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.pengpengdd.cyou/gtpmsaovag.html

[T55] Scala：集合过滤
来源：http://hz.zhengqikj.top/gthuuymszl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.tianlin.xyz/gtsphjdybg.html

[T56] Scala：样例类
来源：http://hz.zhixingplan.top/gtefsysjrp.html

case class User(name: String, age: Int)
来源：http://hz.shanyushiyangkeji.top/gtiojuedml.html

[T57] Scala：模式匹配
来源：http://hz.haohaochexian.top/gtuyhsrpaa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ivvv.top/gtspmciykh.html

[T58] Scala：函数定义
来源：http://hz.chenzaomai.com/gtzinizptd.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yueranfly.top/gtbolrpqvz.html

[T59] Scala：循环
来源：http://hz.wangdashe.top/gtlfjcsvnh.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenzaomai.com/gtphlpfsjm.html

[T60] Scala：折叠
来源：http://hz.guowangkeji.top/gtarvxhmnj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xuetiantiany.cn/gtmltidrhe.html

================================================================================
来源：http://hz.snrcjt.cn/gtfgtsodae.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuanzhike.top/gtipyobylq.html

================================================================================
来源：http://hz.gotoacloud.top/gtduvcniqk.html

[U01] Py：创建虚拟环境
来源：http://hz.yangfankeji.com/gtzcpycgdc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ivvv.top/gteubwybhk.html

[U02] Py：导出 / 安装依赖
来源：http://hz.mhx1999.top/gtcgrwuxfo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cqqwz.cn/gtuusimpur.html

[U03] Py：加载 .env 配置
来源：http://hz.nwbrower.top/gtrjssntwj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jinyuanbaomall.cn/gtmqfkobtr.html

[U04] Py：变量调试打印
来源：http://hz.aizwys.cn/gthrhogmml.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.guannengcc.top/gthqksycxt.html

[U05] Py：列表去重且保序
来源：http://hz.hammf.cn/gtobzbgnxg.html

list(dict.fromkeys(arr))
来源：http://hz.chenlongwang.top/gtkplsfrdk.html

[U06] Py：合并两个字典
来源：http://hz.daxiang520.top/gtmqpnlspc.html

{**a, **b}
来源：http://hz.jyoumei.cn/gtzitviuha.html

[U07] Py：反转字典键值
来源：http://hz.gogol.net.cn/gtbgxhunys.html

{v: k for k, v in d.items()}
来源：http://hz.dashuyun.cn/gtlzishuec.html

[U08] Py：展平二维列表
来源：http://hz.9152youxi.cn/gtdszbqkhs.html

[y for x in nested for y in x]
来源：http://hz.cucudq.cn/gtaspjxqjb.html

[U09] Py：字典取最大值的键
来源：http://hz.cashguo.top/gtgaukuflk.html

max(d, key=d.get)
来源：http://hz.xuanzx.com/gtabdyksgb.html

[U10] Py：按值排序字典
来源：http://hz.jinghuilouyu.cn/gtvkwryzqz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cashguo.top/gtkpijdkay.html

[U11] Py：生成器表达式
来源：http://hz.xinyue.icu/gtarmbjxas.html

(x * 2 for x in arr)
来源：http://hz.quarkkingdee.top/gtuoulyhyx.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cdnleiting.top/gtderttmyv.html

Counter(arr).most_common(3)
来源：http://hz.yj202588.top/gtlurkwytw.html

[U13] Py：固定长度队列
来源：http://hz.shuidangran.top/gtbkunraob.html

deque(maxlen=10)
来源：http://hz.zycfv.cn/gtdrgulrln.html

[U14] Py：分组收集到列表
来源：http://hz.hammf.cn/gtgjkcdfss.html

defaultdict(list)
来源：http://hz.tanke756.top/gtdxrhmqin.html

[U15] Py：高精度计时
来源：http://hz.hnqzz.top/gtzctrdfva.html

t = time.perf_counter()
来源：http://hz.gzhubu.top/gtldyzyofk.html

[U16] Py：命令行参数解析
来源：http://hz.smart0.xyz/gtpryfqlpt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xylfe.cn/gtlmsuobdh.html

[U17] Py：初始化日志
来源：http://hz.smart0.xyz/gtqakdpmws.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jinghuilouyu.cn/gtmsmewltk.html

[U18] Py：预编译正则
来源：http://hz.chenjidiqi.icu/gtjfzmlpno.html

pat = re.compile(r"\d+")
来源：http://hz.nwbrower.top/gthjnetrgw.html

[U19] Py：正则替换带回调
来源：http://hz.dashuyun.cn/gtdtaczmoi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhaomingkeji.xyz/gttgdckzcw.html

[U20] Py：缓存函数结果
来源：http://hz.ppjwa.cn/gtiagogvvv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.svipenyu.cn/gthsoibyem.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhiwuduotai.top/gtiwbbgyig.html

@contextlib.contextmanager
来源：http://hz.yj20258.top/gtboncwkcr.html

[U22] Py：矩阵转置
来源：http://hz.zhiwuduotai.top/gtmekpqdkr.html

list(zip(*m))
来源：http://hz.tanke756.top/gtrgqgrjei.html

[U23] Py：分块读取大文件
来源：http://hz.yj20258.top/gtofucjetk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xingfuxueyuan.xyz/gtcwynefzf.html

[U24] Py：路径操作
来源：http://hz.nanxuanxn.top/gtpiveojov.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hysaishi.cn/gtxovktipf.html

[U25] Py：CSV 按字典读
来源：http://hz.zhaomingkeji.xyz/gteigoznhy.html

csv.DictReader(f)
来源：http://hz.wangdashe.top/gtejaayyds.html

[U26] Py：并发下载
来源：http://hz.daria6918.cn/gtvbldbdzx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hnxiangtu.top/gtetgpdmvo.html

[U27] Py：异步 HTTP
来源：http://hz.yj20258.top/gtokaqezsr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yj20258888.top/gtdjpblmdj.html

[U28] Py：类型别名
来源：http://hz.zhixingplan.top/gtddqyymwi.html

UserId = int
来源：http://hz.xuanzx.com/gtcksnhfvy.html

[U29] Py：属性校验
来源：http://hz.cashguo.top/gtsczaidyu.html

@property 与 @x.setter 配合
来源：http://hz.hongshengwenyu.top/gtisvsylpy.html

[U30] Py：数据类
来源：http://hz.52xcode.cn/gtpzhgwkta.html

@dataclass(slots=True)
来源：http://hz.zhoulong.xyz/gtqqgtccxd.html

[U31] Py：单测
来源：http://hz.dianchejie.cn/gtqtxbwrcz.html

python -m pytest -q
来源：http://hz.zhijiandao.cn/gtjemsuxlh.html

[U32] Py：代码格式化
来源：http://hz.jinqigfzy.top/gtfhupizlb.html

ruff format . && ruff check --fix .
来源：http://hz.yj20258888.top/gtswgpwqst.html

[U33] Py：打包发布
来源：http://hz.smart0.xyz/gtigmvnnrr.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yj20258888.top/gteiscbvec.html

[U34] Py：判断编码
来源：http://hz.nwbrower.top/gtvlvsrksf.html

chardet.detect(raw)
来源：http://hz.guowangkeji.top/gttilfixvg.html

[U35] Py：发送邮件
来源：http://hz.zhoulong.xyz/gtmmpbzkgq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shangyingyoupin.top/gthddhbdrr.html

[U36] Py：定时任务
来源：http://hz.xylfe.cn/gtxbbztusg.html

schedule.every(10).minutes.do(job)
来源：http://hz.gaohongyu789.top/gtoogzodqx.html

[U37] Py：读写 Excel
来源：http://hz.cheryme.top/gtmwytamhp.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinqigfzy.top/gtkpaummdf.html

[U38] Py：获取脚本所在目录
来源：http://hz.shangyingyoupin.top/gtponbqklt.html

Path(__file__).resolve().parent
来源：http://hz.jinqigufen.top/gtuhbqkjce.html

[U39] Py：判断是否在交互环境
来源：http://hz.0kj1m.cn/gthximbnib.html

sys.stdout.isatty()
来源：http://hz.316326.xyz/gtubdfjldr.html

[U40] Py：打印到标准错误
来源：http://hz.jqgufenzy.top/gtxskufbhz.html

print("err", file=sys.stderr)
来源：http://hz.cdnleiting.top/gtxdxgkfvn.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shanyushiyangtech.top/gtkiiowfvh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhiwuduotai.top/gttevefggb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sxryk.cn/gtkqovvmhx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.sufxvd.cn/gtgfoktktl.html

[U43] PHP：声明命名空间
来源：http://hz.yueranfly.top/gtulcuiwax.html

namespace App\Http;
来源：http://hz.jianghu66.top/gtrrmmkyom.html

[U44] PHP：开启严格类型
来源：http://hz.hfpthk.cn/gtnhkngxlp.html

declare(strict_types=1);
来源：http://hz.jqgfzy.top/gtprhqjvpi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.fzhhl.top/gtlkeltdaw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtejaaqjsk.html

[U46] PHP：可空类型
来源：http://hz.shzxlz.cn/gtictskhul.html

?string $name = null
来源：http://hz.daxiang520.top/gtwrzmpdyq.html

[U47] PHP：联合类型
来源：http://hz.hfpthk.cn/gtxruykfgs.html

int|string $id
来源：http://hz.zhoulong.xyz/gtgwgzxrsd.html

[U48] PHP：纯枚举
来源：http://hz.ppjwa.cn/gtqtdqfjow.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhiwuduotai.top/gtflbnvzuc.html

[U49] PHP：只读属性
来源：http://hz.hnxiangtu.top/gtlgeajaan.html

public readonly string $name
来源：http://hz.smart0.xyz/gtyjpcvhch.html

[U50] PHP：构造器属性提升
来源：http://hz.jqgfzy.top/gtyigbqwyn.html

public function __construct(private int $id) {}
来源：http://hz.redwolf501.top/gtwqwzsxjh.html

[U51] PHP：数组解构
来源：http://hz.daxiang520.top/gtdasucobz.html

[$a, $b] = $arr;
来源：http://hz.hnqzz.top/gtryriwsnz.html

[U52] PHP：箭头函数
来源：http://hz.jinyuanbaomall.cn/gtwzyowxty.html

$double = fn($x) => $x * 2;
来源：http://hz.zhengqikj.top/gtxwfgdzso.html

[U53] PHP：空合并运算符
来源：http://hz.0kj1m.cn/gtmnsjaubi.html

$v = $a ?? $b ?? "default";
来源：http://hz.yangfankeji.com/gtfibtsryv.html

[U54] PHP：空安全调用
来源：http://hz.tanke756.top/gtcazmokjf.html

$obj?->method()
来源：http://hz.jqgfzy.top/gtbxrdbmxi.html

[U55] PHP：match 表达式
来源：http://hz.jyoumei.cn/gtszupkqmm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jlsjyb.cn/gtfcyczewz.html

[U56] PHP：命名参数
来源：http://hz.jinqigfzy.top/gttjdemryb.html

f(a: 1, b: 2)
来源：http://hz.yuxming.cn/gtltbzetxc.html

[U57] PHP：字符串插值
来源：http://hz.meibo888.top/gtcqvqhlzi.html

"值: {$a}"
来源：http://hz.sxryk.cn/gtgwldvbwg.html

[U58] PHP：数组三件套
来源：http://hz.svipenyu.cn/gtlkntekoq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cqqwz.cn/gtfxjqsfyq.html

[U59] PHP：自定义排序
来源：http://hz.yongpay.top/gtwckctbjx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tanke756.top/gtpvllxgzj.html

[U60] PHP：JSON 编解码
来源：http://hz.0kj1m.cn/gtqwjsskeb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hammf.cn/gteqdilykd.html

[U61] PHP：正则
来源：http://hz.hfpthk.cn/gtjntcpkxq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhongyouzk.top/gttfxjqzgh.html

[U62] PHP：日期对象
来源：http://hz.tanke756.top/gtrqmtymfu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.bjfxy.top/gtixvwygcl.html

[U63] PHP：文件读写
来源：http://hz.yonumen.top/gttqmfmgos.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shanyushiyangtech.top/gtrgwcyjpl.html

[U64] PHP：目录遍历
来源：http://hz.haohaochexian.top/gtvjjnslxl.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yuanzhike.top/gtrazhtnpg.html

[U65] PHP：会话
来源：http://hz.yangfankeji.com/gtdawvdlwn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.bjfxy.top/gteolxeedh.html

[U66] PHP：设置 Cookie
来源：http://hz.shanyushiyangtech.top/gtgfyubyvs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yueranfly.top/gtupactseo.html

[U67] PHP：处理文件上传
来源：http://hz.hongshengwenyu.top/gtunnjyssm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yangfankeji.com/gtqjyzxgjx.html

[U68] PHP：PDO 连接
来源：http://hz.sxryk.cn/gtxsksefjf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhaomingkeji.xyz/gthzeubjia.html

[U69] PHP：PDO 预处理
来源：http://hz.jyoumei.cn/gtfikzhmav.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.tian-w.cn/gtsesfsoje.html

[U70] PHP：PDO 事务
来源：http://hz.tian-w.cn/gtdsaaacjs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.havefunace.top/gtjigtowqr.html

[U71] PHP：抛出异常
来源：http://hz.aizwys.cn/gtgzafmmio.html

throw new RuntimeException("失败", 500);
来源：http://hz.nanxinkj.top/gtxdcuaikk.html

[U72] PHP：写错误日志
来源：http://hz.hammf.cn/gtnqpdtxjv.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gzhubu.top/gtwfoqfwes.html

[U73] PHP：读取 ini 配置
来源：http://hz.yonumen.top/gttcesyfau.html

parse_ini_file("config.ini", true)
来源：http://hz.daria6918.cn/gtuijzozyj.html

[U74] PHP：读取环境变量
来源：http://hz.sufxvd.cn/gtjrqshflw.html

getenv("APP_ENV") ?: "production"
来源：http://hz.nwbrower.top/gtrnecgjlc.html

[U75] PHP：依赖注入
来源：http://hz.svipenyu.cn/gtpwdbjtpf.html

composer require psr/container
来源：http://hz.ppjwa.cn/gtqroatxap.html

[U76] PHP：简单路由
来源：http://hz.yuxming.cn/gtpmchtxou.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.xylfe.cn/gtofwostiu.html

[U77] PHP：模板渲染
来源：http://hz.cdnleiting.top/gtvhawlcxh.html

composer require twig/twig
来源：http://hz.gogol.net.cn/gtdbifzmrh.html

[U78] PHP：单元测试
来源：http://hz.ivvv.top/gtynhwqcaj.html

composer require --dev phpunit/phpunit
来源：http://hz.hnqzz.top/gtykoqylbo.html

[U79] PHP：静态分析
来源：http://hz.zhijiandao.cn/gtqcgapuqf.html

composer require --dev phpstan/phpstan
来源：http://hz.svipenyu.cn/gtmyygymmu.html

[U80] PHP：代码规范修复
来源：http://hz.tian-w.cn/gtcuehgdwd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.shuidangran.top/gtnytxihhz.html


<!-- 参考信息 -->