代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj20258888.top/gthfcbefzg.html

[S57] C++：编译期常量
来源：http://hz.hnxiangtu.top/gtpxkyqnsq.html

constexpr int N = 10;
来源：http://hz.hammf.cn/gtwtwydmdq.html

[S58] C++：命名空间
来源：http://hz.haohaochexian.top/gtqjjkktub.html

namespace ns { int f() { return 1; } }
来源：http://hz.quarkkingdee.top/gtbgyhxmty.html

[S59] C++：静态断言
来源：http://hz.feifeiyinyue.top/gtlcunipdg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ivvv.top/gtunutnqvp.html

[S60] C++：遍历并删除元素
来源：http://hz.zhixingplan.top/gtotcqgpgh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenjidiqi.icu/gtlyhziuue.html

================================================================================
来源：http://hz.sweek.top/gtrhkspwcg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinyuanbaomall.cn/gtqcfandmm.html

================================================================================
来源：http://hz.nwbrower.top/gtyzchmaua.html

[T01] Kotlin：Hello World
来源：http://hz.chenjidiqi.icu/gtgitxuruh.html

println("Hello")
来源：http://hz.52xcode.cn/gtmxxspeue.html

[T02] Kotlin：变量
来源：http://hz.sxryk.cn/gtwirhlxyv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cqqwz.cn/gtvuatnvxu.html

[T03] Kotlin：字符串模板
来源：http://hz.guowangkeji.top/gtwhsymyia.html

"值: $b"
来源：http://hz.daxiang520.top/gtzbugewgp.html

[T04] Kotlin：空安全
来源：http://hz.yj20258.top/gttyctoymx.html

val n: String? = null;  n?.length
来源：http://hz.jqgufenzy.top/gtcipxaarz.html

[T05] Kotlin：when 表达式
来源：http://hz.zhiwuduotai.top/gtrgdvcbhl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xuanzx.com/gtqdbyuwan.html

[T06] Kotlin：集合映射
来源：http://hz.chenlongwang.top/gtcjkjmzet.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ehwqpu.com/gtgyrojncm.html

[T07] Kotlin：集合过滤
来源：http://hz.c1oappe.top/gtuvvcbnko.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cheryme.top/gtsntjmksq.html

[T08] Kotlin：数据类
来源：http://hz.gotoacloud.top/gtrjdueppi.html

data class User(val name: String, val age: Int)
来源：http://hz.chenzaomai.com/gtbbwwyhyl.html

[T09] Kotlin：扩展函数
来源：http://hz.316326.xyz/gtavbrkvxj.html

fun String.exclaim() = this + "!"
来源：http://hz.ydjk.org.cn/gtrmbuxpux.html

[T10] Kotlin：默认参数
来源：http://hz.guowangkeji.top/gthgnqagzu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yongpay.top/gtcptqcqtl.html

[T11] Kotlin：协程
来源：http://hz.shuidangran.top/gtoxvhdpch.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhoulong.xyz/gtrsyugiaq.html

[T12] Kotlin：解构声明
来源：http://hz.zhengqikj.top/gtcsvfbxpa.html

val (a, b) = Pair(1, 2)
来源：http://hz.zdqjudy.top/gtgqyycnmy.html

[T13] Kotlin：只读 Map
来源：http://hz.zycfv.cn/gtmxwtqhti.html

val m = mapOf("a" to 1)
来源：http://hz.birdmap.top/gtsbqpctxy.html

[T14] Kotlin：循环
来源：http://hz.hammf.cn/gtqqrjfoym.html

for (i in 1..10) println(i)
来源：http://hz.tanke756.top/gtosxndxik.html

[T15] Kotlin：接口
来源：http://hz.jlsjyb.cn/gtmcabuqet.html

interface Shape { fun area(): Double }
来源：http://hz.kuanghao11.cn/gtpvnmasjt.html

[T16] Swift：Hello World
来源：http://hz.zycfv.cn/gtghrhrzhq.html

print("Hello")
来源：http://hz.chenzaomai.com/gtedxmytkh.html

[T17] Swift：变量与常量
来源：http://hz.yangfankeji.com/gtelhuvwbl.html

var a = 1;  let b = 2
来源：http://hz.sxryk.cn/gtcklonins.html

[T18] Swift：字符串插值
来源：http://hz.ppjwa.cn/gtzxjvmjsv.html

"值: \(b)"
来源：http://hz.9152youxi.cn/gtlqvveklq.html

[T19] Swift：可选绑定
来源：http://hz.yj20258888.top/gtleeqtual.html

if let n = opt { print(n) }
来源：http://hz.xuetiantiany.cn/gtmdbtswno.html

[T20] Swift：数组操作
来源：http://hz.pengpengdd.cyou/gtexmsqull.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daxiang520.top/gtjwmnmkmf.html

[T21] Swift：遍历
来源：http://hz.wangdashe.top/gtjwukdsgk.html

for x in a { print(x) }
来源：http://hz.yuanzhike.top/gtjadtgizb.html

[T22] Swift：字典
来源：http://hz.jianghu66.top/gtztkvcenj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.pengpengdd.cyou/gtxeamnksy.html

[T23] Swift：函数
来源：http://hz.gotoacloud.top/gtxesnxwqb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.birdmap.top/gtsaeupndl.html

[T24] Swift：闭包
来源：http://hz.haohaochexian.top/gteyrcjvis.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.vqdsnc.cn/gtyqlnpfoj.html

[T25] Swift：结构体
来源：http://hz.tianlin.xyz/gtdgnnazoy.html

struct P { var x: Int }
来源：http://hz.xylfe.cn/gtltzekypl.html

[T26] Swift：类与重写
来源：http://hz.yueranfly.top/gtrytzzqer.html

class A: Base { override func f() {} }
来源：http://hz.xuanzx.com/gtorhxmzet.html

[T27] Swift：错误处理
来源：http://hz.yongpay.top/gtacxzpekj.html

do { try f() } catch { print(error) }
来源：http://hz.zhijiandao.cn/gteooibtkq.html

[T28] Swift：枚举
来源：http://hz.gaohongyu789.top/gtpxydrcak.html

enum Color { case red, green }
来源：http://hz.jinqigfzy.top/gtnwlugcer.html

[T29] Swift：guard 提前返回
来源：http://hz.gogol.net.cn/gtgumwwoee.html

guard let x = opt else { return }
来源：http://hz.jinyuanbaomall.cn/gthzsdkplo.html

[T30] Swift：协议
来源：http://hz.jqgufenzy.top/gtiehlaind.html

protocol Shape { func area() -> Double }
来源：http://hz.cdnleiting.top/gtpxremxhf.html

[T31] Lua：Hello World
来源：http://hz.daxiang520.top/gtumownomg.html

print("Hello")
来源：http://hz.jianghu66.top/gtxusaigpn.html

[T32] Lua：局部变量
来源：http://hz.meibo888.top/gtukjwoosc.html

local a = 1
来源：http://hz.birdmap.top/gtuxwdbwtd.html

[T33] Lua：表（数组）
来源：http://hz.nanxuanxn.top/gtdkxsdfbl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhijiandao.cn/gtttgsjknb.html

[T34] Lua：遍历表
来源：http://hz.c1oappe.top/gtonqocigs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.pycfn.com/gtpwxtqpqa.html

[T35] Lua：字典表
来源：http://hz.daxiang520.top/gtxkjhqhpt.html

local d = { a = 1 };  d.b = 2
来源：http://hz.bjfxy.top/gtjkoukzyx.html

[T36] Lua：函数
来源：http://hz.haohaochexian.top/gtwfrwqyrt.html

function add(a, b) return a + b end
来源：http://hz.chenzaomai.com/gtiaklbvmr.html

[T37] Lua：字符串拼接
来源：http://hz.shangyingyoupin.top/gtkzkgnhtg.html

"a" .. "b"
来源：http://hz.birdmap.top/gtzfsobqht.html

[T38] Lua：条件
来源：http://hz.gaohongyu789.top/gtbfmkxmvb.html

if x > 0 then print("正") end
来源：http://hz.zhengqikj.top/gtrvjkioux.html

[T39] Lua：模式匹配
来源：http://hz.vqdsnc.cn/gtyudhdqtb.html

string.find(s, "%d+")
来源：http://hz.iojbl.cn/gtdhecqfnt.html

[T40] Lua：元表
来源：http://hz.yj20258888.top/gttkftuyii.html

setmetatable({}, { __index = base })
来源：http://hz.chenjidiqi.icu/gtrehlngtp.html

[T41] Perl：Hello World
来源：http://hz.cheryme.top/gtqmaozqxy.html

print "Hello\n";
来源：http://hz.yj202588.top/gtrhjzlunv.html

[T42] Perl：变量类型
来源：http://hz.0kj1m.cn/gteixrbaft.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gogol.net.cn/gtlbkiedcm.html

[T43] Perl：字符串插值
来源：http://hz.haohaochexian.top/gtpblseedp.html

"值: $a"
来源：http://hz.gotoacloud.top/gtkcrcjgph.html

[T44] Perl：条件
来源：http://hz.sufxvd.cn/gtfekdcckz.html

if ($a > 0) { print "正"; }
来源：http://hz.shanyushiyangtech.top/gtjnncpdey.html

[T45] Perl：数组遍历
来源：http://hz.snrcjt.cn/gtxtmyiati.html

for my $x (@arr) { print $x; }
来源：http://hz.jqgfzy.top/gtdbcumjzx.html

[T46] Perl：哈希操作
来源：http://hz.yanxiufei.cn/gtkdypjhxw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhijiandao.cn/gtojrotutr.html

[T47] Perl：正则捕获
来源：http://hz.yuxming.cn/gtscnxawoq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ppjwa.cn/gtsphqcriu.html

[T48] Perl：正则替换
来源：http://hz.iojbl.cn/gtwfouonlf.html

$s =~ s/old/new/g;
来源：http://hz.smart0.xyz/gtnvpxijgi.html

[T49] Perl：函数
来源：http://hz.yj20258888.top/gtxnzspqlt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ywan-chungtsiang.top/gtyeupjtbm.html

[T50] Perl：逐行读文件
来源：http://hz.gogol.net.cn/gtqlucpfft.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cheryme.top/gtxrqvyynh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xinyue.icu/gtbaddugiy.html

[T51] Scala：Hello World
来源：http://hz.svipenyu.cn/gtrknxmqwt.html

println("Hello")
来源：http://hz.sysykeji.top/gtpzbrmagd.html

[T52] Scala：变量
来源：http://hz.xuetiantiany.cn/gtcvijinwb.html

val a = 1;  var b = 2
来源：http://hz.jlsjyb.cn/gtkrjvdvpl.html

[T53] Scala：字符串插值
来源：http://hz.zhixingplan.top/gtjqhoomiw.html

s"值: $b"
来源：http://hz.daria6918.cn/gtvdfgmmnn.html

[T54] Scala：集合映射
来源：http://hz.nwbrower.top/gteajusmgp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shangyingyoupin.top/gtxwzgzsmn.html

[T55] Scala：集合过滤
来源：http://hz.hfpthk.cn/gtfourzsre.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.smart0.xyz/gtsaqapbdx.html

[T56] Scala：样例类
来源：http://hz.xinyue.icu/gtrrwqkeck.html

case class User(name: String, age: Int)
来源：http://hz.yj20258.top/gtnuvchpyo.html

[T57] Scala：模式匹配
来源：http://hz.zdqjudy.top/gtsnwuqrat.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yj20258888.top/gtcjznzouo.html

[T58] Scala：函数定义
来源：http://hz.xziqi.cn/gtmdwodpsa.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sysykeji.top/gtkrjnnhgu.html

[T59] Scala：循环
来源：http://hz.0kj1m.cn/gtpcukgqin.html

for (i <- 1 to 10) println(i)
来源：http://hz.sufxvd.cn/gtlevkmzqs.html

[T60] Scala：折叠
来源：http://hz.0kj1m.cn/gtagpfpxvl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.aizwys.cn/gtuvmtkwwe.html

================================================================================
来源：http://hz.gogol.net.cn/gtatsejhtw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ivvv.top/gtvcuuhwci.html

================================================================================
来源：http://hz.xuanzx.com/gtlvbcydon.html

[U01] Py：创建虚拟环境
来源：http://hz.xuetiantiany.cn/gtyeorblvs.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shanyushiyangtech.top/gtkwcwyvyb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.c1oappe.top/gtjhtlinbn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ybcxt.top/gtjlpnjgeh.html

[U03] Py：加载 .env 配置
来源：http://hz.smart0.xyz/gtjhjbcbpu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhongyouzk.top/gtescqtice.html

[U04] Py：变量调试打印
来源：http://hz.c1oappe.top/gtlhxltqng.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ydzc1.top/gtinfvfesj.html

[U05] Py：列表去重且保序
来源：http://hz.jlsjyb.cn/gtzulhqvuo.html

list(dict.fromkeys(arr))
来源：http://hz.52xcode.cn/gtggyzkzkz.html

[U06] Py：合并两个字典
来源：http://hz.daxiang520.top/gtoruixytp.html

{**a, **b}
来源：http://hz.sxryk.cn/gtthtnyjfa.html

[U07] Py：反转字典键值
来源：http://hz.zhixingplan.top/gteedztxtq.html

{v: k for k, v in d.items()}
来源：http://hz.c1oappe.top/gtalcbxueo.html

[U08] Py：展平二维列表
来源：http://hz.jinghuilouyu.cn/gtixxswsyb.html

[y for x in nested for y in x]
来源：http://hz.hysaishi.cn/gtwdtopasj.html

[U09] Py：字典取最大值的键
来源：http://hz.daria6918.cn/gtzxabfrop.html

max(d, key=d.get)
来源：http://hz.52xcode.cn/gtpjqmniau.html

[U10] Py：按值排序字典
来源：http://hz.0kj1m.cn/gtagamcbye.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xylfe.cn/gtspdtpuop.html

[U11] Py：生成器表达式
来源：http://hz.wangshuangyany.cn/gtbqtjucnt.html

(x * 2 for x in arr)
来源：http://hz.jinqigfzy.top/gtsrfvfbxj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.snrcjt.cn/gtsxwpollc.html

Counter(arr).most_common(3)
来源：http://hz.xziqi.cn/gtkakzsxdx.html

[U13] Py：固定长度队列
来源：http://hz.jinyuanbaomall.cn/gthukvawdj.html

deque(maxlen=10)
来源：http://hz.xylfe.cn/gtfgzoucys.html

[U14] Py：分组收集到列表
来源：http://hz.sweek.top/gtrcatxddb.html

defaultdict(list)
来源：http://hz.jiagoushi.top/gtompcrzsb.html

[U15] Py：高精度计时
来源：http://hz.9152youxi.cn/gtrkhcobgg.html

t = time.perf_counter()
来源：http://hz.meibo888.top/gtjbcjxpig.html

[U16] Py：命令行参数解析
来源：http://hz.fengsongda.top/gtqqtubbcv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yangfankeji.com/gtxzxsqvjm.html

[U17] Py：初始化日志
来源：http://hz.wangdashe.top/gtacovzqvx.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.daria6918.cn/gtionbnucm.html

[U18] Py：预编译正则
来源：http://hz.ywan-chungtsiang.top/gtkmbtutbb.html

pat = re.compile(r"\d+")
来源：http://hz.havefunace.top/gtlmqydtnq.html

[U19] Py：正则替换带回调
来源：http://hz.svipenyu.cn/gthqgnndlu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hywenlv.cn/gtlkpazckk.html

[U20] Py：缓存函数结果
来源：http://hz.shangyingyoupin.top/gtmuhnpyky.html

@functools.lru_cache(maxsize=None)
来源：http://hz.c1oappe.top/gtocnwpdkq.html

[U21] Py：自定义上下文管理器
来源：http://hz.xingfuxueyuan.xyz/gtrvikuxmh.html

@contextlib.contextmanager
来源：http://hz.jyoumei.cn/gtiqnlcqnl.html

[U22] Py：矩阵转置
来源：http://hz.wangshuangyany.cn/gtvjlxbmst.html

list(zip(*m))
来源：http://hz.fengsongda.top/gtjtqdduki.html

[U23] Py：分块读取大文件
来源：http://hz.hongshengwenyu.top/gtphqsogok.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.pycfn.com/gtnrfaukyg.html

[U24] Py：路径操作
来源：http://hz.sweek.top/gtftdscddb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gogol.net.cn/gtdhlmwxom.html

[U25] Py：CSV 按字典读
来源：http://hz.tianlin.xyz/gtqmpbwwio.html

csv.DictReader(f)
来源：http://hz.jinghuilouyu.cn/gtzpstxyaz.html

[U26] Py：并发下载
来源：http://hz.kuanghao11.cn/gtzimgrfah.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jqgfzy.top/gtbgwhqgdy.html

[U27] Py：异步 HTTP
来源：http://hz.svipenyu.cn/gtnbfkggva.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.svipenyu.cn/gtmprdkpxw.html

[U28] Py：类型别名
来源：http://hz.yuxming.cn/gtcpwyghvh.html

UserId = int
来源：http://hz.hongshengwenyu.top/gtqwylpxln.html

[U29] Py：属性校验
来源：http://hz.gzhubu.top/gtsiidnrhi.html

@property 与 @x.setter 配合
来源：http://hz.jinqigufen.top/gtoicnnlfz.html

[U30] Py：数据类
来源：http://hz.shzxlz.cn/gtnraipqxe.html

@dataclass(slots=True)
来源：http://hz.meibo888.top/gtatafxezr.html

[U31] Py：单测
来源：http://hz.shuidangran.top/gtdaqmeeye.html

python -m pytest -q
来源：http://hz.yuanzhike.top/gtycyqcstq.html

[U32] Py：代码格式化
来源：http://hz.shanyushiyangkeji.top/gtusuxmlax.html

ruff format . && ruff check --fix .
来源：http://hz.svipenyu.cn/gtaujlltks.html

[U33] Py：打包发布
来源：http://hz.hongshengwenyu.top/gtymyvvwvm.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.nwbrower.top/gtbpntxjzx.html

[U34] Py：判断编码
来源：http://hz.yongpay.top/gtshholgya.html

chardet.detect(raw)
来源：http://hz.sufxvd.cn/gthjsboeec.html

[U35] Py：发送邮件
来源：http://hz.zhongyouzk.top/gtdtkxtowe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nanxinkj.top/gtnowapicv.html

[U36] Py：定时任务
来源：http://hz.birdmap.top/gteccgdtvc.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj202588.top/gthypsvfax.html

[U37] Py：读写 Excel
来源：http://hz.ivvv.top/gtooojdkpu.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zycfv.cn/gtqevookws.html

[U38] Py：获取脚本所在目录
来源：http://hz.feifeiyinyue.top/gtdpwfqiss.html

Path(__file__).resolve().parent
来源：http://hz.hongshengwenyu.top/gtrghjrhqy.html

[U39] Py：判断是否在交互环境
来源：http://hz.aibaodan.cn/gtepxxvtjm.html

sys.stdout.isatty()
来源：http://hz.gogol.net.cn/gtghckdjdx.html

[U40] Py：打印到标准错误
来源：http://hz.xuetiantiany.cn/gtasjcejfw.html

print("err", file=sys.stderr)
来源：http://hz.jinqigufen.top/gtmwnhctre.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hfpthk.cn/gtqylamqfz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.kuanghao11.cn/gtvnycsoas.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenzaomai.com/gtpsbeaetu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hongshengwenyu.top/gtaexeqqpv.html

[U43] PHP：声明命名空间
来源：http://hz.xylfe.cn/gtcbcvbzne.html

namespace App\Http;
来源：http://hz.zhaomingkeji.xyz/gtwwfczqcu.html

[U44] PHP：开启严格类型
来源：http://hz.jinqigufen.top/gtjsgflisd.html

declare(strict_types=1);
来源：http://hz.316326.xyz/gthjmeepgg.html

[U45] PHP：类型声明与返回类型
来源：http://hz.nwbrower.top/gtogadccul.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jiagoushi.top/gtuxchnxua.html

[U46] PHP：可空类型
来源：http://hz.zycfv.cn/gtnwvtborg.html

?string $name = null
来源：http://hz.wangshuangyany.cn/gtmsxqblre.html

[U47] PHP：联合类型
来源：http://hz.hysaishi.cn/gtmeyudhnr.html

int|string $id
来源：http://hz.0kj1m.cn/gtzfqrjuna.html

[U48] PHP：纯枚举
来源：http://hz.chenjidiqi.icu/gtbuntcceg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gaohongyu789.top/gtkjnzculn.html

[U49] PHP：只读属性
来源：http://hz.xziqi.cn/gtakaqazkj.html

public readonly string $name
来源：http://hz.chenjidiqi.icu/gtdfohbgyr.html

[U50] PHP：构造器属性提升
来源：http://hz.jqgufenzy.top/gtywnxctri.html

public function __construct(private int $id) {}
来源：http://hz.jlsjyb.cn/gtdxvymjdl.html

[U51] PHP：数组解构
来源：http://hz.daria6918.cn/gtfvllkrwq.html

[$a, $b] = $arr;
来源：http://hz.sufxvd.cn/gtreiibfaa.html

[U52] PHP：箭头函数
来源：http://hz.jinqigfzy.top/gttvpmbffy.html

$double = fn($x) => $x * 2;
来源：http://hz.guowangkeji.top/gtjyndsnem.html

[U53] PHP：空合并运算符
来源：http://hz.hysaishi.cn/gtpizmhbxd.html

$v = $a ?? $b ?? "default";
来源：http://hz.yuanzhike.top/gtpaowenhy.html

[U54] PHP：空安全调用
来源：http://hz.zhixingplan.top/gtfcmfzsec.html

$obj?->method()
来源：http://hz.hysaishi.cn/gtqdeexbdi.html

[U55] PHP：match 表达式
来源：http://hz.birdmap.top/gtielbtyso.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cqqwz.cn/gtjdcxmtxh.html

[U56] PHP：命名参数
来源：http://hz.daria6918.cn/gtztcmrohc.html

f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gthmweidhq.html

[U57] PHP：字符串插值
来源：http://hz.iojbl.cn/gtufunayxe.html

"值: {$a}"
来源：http://hz.sysykeji.top/gtfzaefkqn.html

[U58] PHP：数组三件套
来源：http://hz.xinyue.icu/gtcsyvqmkw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.fzhhl.top/gtunuumleo.html

[U59] PHP：自定义排序
来源：http://hz.zhiwuduotai.top/gtxtdglnsl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.feifeiyinyue.top/gtobhqqcob.html

[U60] PHP：JSON 编解码
来源：http://hz.nwbrower.top/gtphbsievw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.meibo888.top/gtirypzxda.html

[U61] PHP：正则
来源：http://hz.sweek.top/gtbfscqrwf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhiwuduotai.top/gtonbeoklz.html

[U62] PHP：日期对象
来源：http://hz.snrcjt.cn/gttaafmnmt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cqqwz.cn/gtikititju.html

[U63] PHP：文件读写
来源：http://hz.zycfv.cn/gtcpwosepx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cashguo.top/gtfnvthjly.html

[U64] PHP：目录遍历
来源：http://hz.xuanzx.com/gtsdmsubce.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ivvv.top/gtjfjbeakw.html

[U65] PHP：会话
来源：http://hz.sufxvd.cn/gtwpsysoww.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zycfv.cn/gtlpndnmcq.html

[U66] PHP：设置 Cookie
来源：http://hz.jianghu66.top/gtfiwsrnhy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ppjwa.cn/gtxkimstrr.html

[U67] PHP：处理文件上传
来源：http://hz.zhaomingkeji.xyz/gtximwhucf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.svipenyu.cn/gtaphhivis.html

[U68] PHP：PDO 连接
来源：http://hz.smart0.xyz/gtpymytkgs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.sweek.top/gttvimlntg.html

[U69] PHP：PDO 预处理
来源：http://hz.xinyue.icu/gtfwyrnwyw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.havefunace.top/gtrtiuhkon.html

[U70] PHP：PDO 事务
来源：http://hz.zhijiandao.cn/gtsvgvywql.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cdnleiting.top/gtvcwryinj.html

[U71] PHP：抛出异常
来源：http://hz.shuidangran.top/gtukdnwiqm.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhijiandao.cn/gtrkcwxqxp.html

[U72] PHP：写错误日志
来源：http://hz.shanyushiyangkeji.top/gtjfnrknzl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.sxryk.cn/gtaevmgpdl.html

[U73] PHP：读取 ini 配置
来源：http://hz.ydjk.org.cn/gtgyvuxnif.html

parse_ini_file("config.ini", true)
来源：http://hz.yj20258.top/gtsicljupl.html

[U74] PHP：读取环境变量
来源：http://hz.hnxiangtu.top/gtcxxuttmn.html

getenv("APP_ENV") ?: "production"
来源：http://hz.sysykeji.top/gtbghvttqe.html

[U75] PHP：依赖注入
来源：http://hz.feifeiyinyue.top/gtmfymuxlw.html

composer require psr/container
来源：http://hz.zycfv.cn/gthfwjqsls.html

[U76] PHP：简单路由
来源：http://hz.jinyuanbaomall.cn/gtnuzgpand.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zdqjudy.top/gtxxycyjao.html

[U77] PHP：模板渲染
来源：http://hz.hnxiangtu.top/gtrqkqxlik.html

composer require twig/twig
来源：http://hz.guannengcc.top/gtvgeyssif.html

[U78] PHP：单元测试
来源：http://hz.hfpthk.cn/gtcfuedewa.html

composer require --dev phpunit/phpunit
来源：http://hz.jinqigufen.top/gtbfxcnkru.html

[U79] PHP：静态分析
来源：http://hz.jiagoushi.top/gtulojqvnf.html

composer require --dev phpstan/phpstan
来源：http://hz.cqqwz.cn/gttyzdspre.html

[U80] PHP：代码规范修复
来源：http://hz.zhengqikj.top/gtwqspplcb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.shanyushiyangtech.top/gtpagfaswv.html

[U81] JS：初始化项目
来源：http://hz.dashuyun.cn/gtoaxjtvcz.html

npm init -y;  npm i express
来源：http://hz.gogol.net.cn/gttksspqnw.html

[U82] JS：package.json 脚本
来源：http://hz.vqdsnc.cn/gtsgcldulx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.pengpengdd.cyou/gtaknzjksz.html


<!-- 参考信息 -->