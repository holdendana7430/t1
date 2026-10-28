代发 wailian999

[S45] C++：lambda
来源：http://hz.yanxiufei.cn/gtpfclkuzb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.vqdsnc.cn/gtpjeqmobm.html

[S46] C++：函数模板
来源：http://hz.cucudq.cn/gtrlcwwmas.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jlsjyb.cn/gtxneqzvgn.html

[S47] C++：结构化绑定遍历
来源：http://hz.svipenyu.cn/gtffdzrsaz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.quarkkingdee.top/gtvcjhgnrm.html

[S48] C++：逐行读文件
来源：http://hz.yj20258.top/gtbwqfzatu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.svipenyu.cn/gtoiqaeaio.html

while (std::getline(in, line)) { }
来源：http://hz.ppjwa.cn/gtuifblnrx.html

[S49] C++：写文件
来源：http://hz.jinghuilouyu.cn/gtteveuodz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xziqi.cn/gtzhzilnjf.html

[S50] C++：格式化数字
来源：http://hz.ywan-chungtsiang.top/gtogveffrk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhixingplan.top/gtbmaqslcj.html

[S51] C++：显式类型转换
来源：http://hz.bjfxy.top/gtdjwxprob.html

static_cast<double>(a) / b
来源：http://hz.jiagoushi.top/gtplblgucs.html

[S52] C++：const 与 noexcept
来源：http://hz.pengpengdd.cyou/gtbsxgmhux.html

int size() const noexcept { return n_; }
来源：http://hz.gogol.net.cn/gtxqggejan.html

[S53] C++：移动语义
来源：http://hz.316326.xyz/gtctegymkf.html

std::vector<int> w = std::move(v);
来源：http://hz.redwolf501.top/gtamltlinc.html

[S54] C++：异常处理
来源：http://hz.smart0.xyz/gtzxqvuudd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yueranfly.top/gtwqgviwbl.html

[S55] C++：结构化绑定
来源：http://hz.aibaodan.cn/gtszvxrbzy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xziqi.cn/gtmnesqewi.html

[S56] C++：optional
来源：http://hz.nwbrower.top/gtumurxklb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shzxlz.cn/gtrktrpzrn.html

[S57] C++：编译期常量
来源：http://hz.chenlongwang.top/gtrrhintom.html

constexpr int N = 10;
来源：http://hz.haohaochexian.top/gtnmdysmge.html

[S58] C++：命名空间
来源：http://hz.hammf.cn/gtbduwkaqp.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhoulong.xyz/gteingvrgb.html

[S59] C++：静态断言
来源：http://hz.9152youxi.cn/gtzruddzpm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.kuanghao11.cn/gteudqblvs.html

[S60] C++：遍历并删除元素
来源：http://hz.dashuyun.cn/gtktnencqw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.aizwys.cn/gtvbpkqoax.html

================================================================================
来源：http://hz.jinqigufen.top/gtkxyewpwj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fzhhl.top/gtclpvnfdn.html

================================================================================
来源：http://hz.daria6918.cn/gtbavpeiiy.html

[T01] Kotlin：Hello World
来源：http://hz.fengsongda.top/gtdazcstpa.html

println("Hello")
来源：http://hz.sxryk.cn/gtwbevlnge.html

[T02] Kotlin：变量
来源：http://hz.yanxiufei.cn/gtylcnzctg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hywenlv.cn/gtgyoteksg.html

[T03] Kotlin：字符串模板
来源：http://hz.jinghuilouyu.cn/gtpkgwuxtz.html

"值: $b"
来源：http://hz.zhoulong.xyz/gtktoviftg.html

[T04] Kotlin：空安全
来源：http://hz.sweek.top/gtspyblhqt.html

val n: String? = null;  n?.length
来源：http://hz.zhixingplan.top/gtfhgvsejz.html

[T05] Kotlin：when 表达式
来源：http://hz.hywenlv.cn/gtbzygeofo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jlsjyb.cn/gtnkwqjekj.html

[T06] Kotlin：集合映射
来源：http://hz.tianlin.xyz/gtsbjkzzvv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.birdmap.top/gtargtgobv.html

[T07] Kotlin：集合过滤
来源：http://hz.andypj.xyz/gtxvcpfzud.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gzhubu.top/gtfjuyctqi.html

[T08] Kotlin：数据类
来源：http://hz.ehwqpu.com/gtsmqfbrvj.html

data class User(val name: String, val age: Int)
来源：http://hz.ehwqpu.com/gtjzfshlsw.html

[T09] Kotlin：扩展函数
来源：http://hz.hnqzz.top/gtekkjhjbk.html

fun String.exclaim() = this + "!"
来源：http://hz.0kj1m.cn/gtyswosxhg.html

[T10] Kotlin：默认参数
来源：http://hz.guannengcc.top/gtdyptkwxb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.fengsongda.top/gtlpfuaxhd.html

[T11] Kotlin：协程
来源：http://hz.cheryme.top/gtynrppbxa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yangfankeji.com/gtupglsoqu.html

[T12] Kotlin：解构声明
来源：http://hz.feifeiyinyue.top/gtnuirzawm.html

val (a, b) = Pair(1, 2)
来源：http://hz.xuetiantiany.cn/gtsinmcohz.html

[T13] Kotlin：只读 Map
来源：http://hz.xziqi.cn/gtuohjezak.html

val m = mapOf("a" to 1)
来源：http://hz.tianlin.xyz/gtgopbjqfz.html

[T14] Kotlin：循环
来源：http://hz.ybcxt.top/gtxkukptvk.html

for (i in 1..10) println(i)
来源：http://hz.hysaishi.cn/gtywbsrhhy.html

[T15] Kotlin：接口
来源：http://hz.316326.xyz/gtuysxvvhp.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gtkgzdaiql.html

[T16] Swift：Hello World
来源：http://hz.gzhubu.top/gtuzbjxjmv.html

print("Hello")
来源：http://hz.9152youxi.cn/gtryjigauu.html

[T17] Swift：变量与常量
来源：http://hz.nanxinkj.top/gtljjkssli.html

var a = 1;  let b = 2
来源：http://hz.iojbl.cn/gtqaiktkni.html

[T18] Swift：字符串插值
来源：http://hz.fzhhl.top/gtioaxuyir.html

"值: \(b)"
来源：http://hz.quarkkingdee.top/gtchposhof.html

[T19] Swift：可选绑定
来源：http://hz.quarkkingdee.top/gtnizqakow.html

if let n = opt { print(n) }
来源：http://hz.yj20258.top/gtmhfjnmmc.html

[T20] Swift：数组操作
来源：http://hz.nwbrower.top/gtedmyujek.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cashguo.top/gtugysndey.html

[T21] Swift：遍历
来源：http://hz.yj20258.top/gttidplwed.html

for x in a { print(x) }
来源：http://hz.yuxming.cn/gtcesjwssa.html

[T22] Swift：字典
来源：http://hz.hongshengwenyu.top/gtisppjwuw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.pycfn.com/gtjseevvdl.html

[T23] Swift：函数
来源：http://hz.jiagoushi.top/gtrohnnvbt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.fengsongda.top/gtifvcazsc.html

[T24] Swift：闭包
来源：http://hz.zhixingplan.top/gtnsifdkqk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.guannengcc.top/gtsiumudbo.html

[T25] Swift：结构体
来源：http://hz.9152youxi.cn/gtuiwpqhjr.html

struct P { var x: Int }
来源：http://hz.jqgufenzy.top/gtgufngbaj.html

[T26] Swift：类与重写
来源：http://hz.iojbl.cn/gtrrvyoxmx.html

class A: Base { override func f() {} }
来源：http://hz.guowangkeji.top/gtgkgxnyai.html

[T27] Swift：错误处理
来源：http://hz.tian-w.cn/gttzrwvjmp.html

do { try f() } catch { print(error) }
来源：http://hz.fzhhl.top/gtzacnxigt.html

[T28] Swift：枚举
来源：http://hz.chenlongwang.top/gtneckqgin.html

enum Color { case red, green }
来源：http://hz.yvedp.cn/gtxjqdkzub.html

[T29] Swift：guard 提前返回
来源：http://hz.hongshengwenyu.top/gtajjhetqm.html

guard let x = opt else { return }
来源：http://hz.yanxiufei.cn/gtuxmtcsaz.html

[T30] Swift：协议
来源：http://hz.cheryme.top/gtfoavmjxp.html

protocol Shape { func area() -> Double }
来源：http://hz.52xcode.cn/gtnuuzfxzq.html

[T31] Lua：Hello World
来源：http://hz.hongshengwenyu.top/gtokokkeot.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtizfexvvh.html

[T32] Lua：局部变量
来源：http://hz.yangfankeji.com/gthiwuquin.html

local a = 1
来源：http://hz.gogol.net.cn/gtwfqhwmzz.html

[T33] Lua：表（数组）
来源：http://hz.quarkkingdee.top/gtlrzenmsp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.chenzaomai.com/gtrisvopcs.html

[T34] Lua：遍历表
来源：http://hz.guowangkeji.top/gtdaeogzap.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.mhx1999.top/gtopnyahxk.html

[T35] Lua：字典表
来源：http://hz.aibaodan.cn/gthmcqyeah.html

local d = { a = 1 };  d.b = 2
来源：http://hz.wangdashe.top/gtamuhzjyv.html

[T36] Lua：函数
来源：http://hz.wangshuangyany.cn/gtjdnmrxhx.html

function add(a, b) return a + b end
来源：http://hz.hnxiangtu.top/gtjbxewmoz.html

[T37] Lua：字符串拼接
来源：http://hz.316326.xyz/gtwexzdnao.html

"a" .. "b"
来源：http://hz.yangfankeji.com/gtwxkpdxog.html

[T38] Lua：条件
来源：http://hz.tian-w.cn/gtkqdgujlv.html

if x > 0 then print("正") end
来源：http://hz.nanxinkj.top/gtxkdujqgp.html

[T39] Lua：模式匹配
来源：http://hz.jqgfzy.top/gtwtdqshln.html

string.find(s, "%d+")
来源：http://hz.hfpthk.cn/gtjcnikgvk.html

[T40] Lua：元表
来源：http://hz.xziqi.cn/gtoucpfupf.html

setmetatable({}, { __index = base })
来源：http://hz.daxiang520.top/gtaeytovjb.html

[T41] Perl：Hello World
来源：http://hz.hammf.cn/gtcdrswurh.html

print "Hello\n";
来源：http://hz.hywenlv.cn/gtrvikmeqh.html

[T42] Perl：变量类型
来源：http://hz.aibaodan.cn/gtyfkvwjza.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.tanke756.top/gtnvuqebva.html

[T43] Perl：字符串插值
来源：http://hz.ivvv.top/gtgnxrvdjj.html

"值: $a"
来源：http://hz.ivvv.top/gtshwovqfy.html

[T44] Perl：条件
来源：http://hz.jinyuanbaomall.cn/gtqsiipdmm.html

if ($a > 0) { print "正"; }
来源：http://hz.aizwys.cn/gtousthbti.html

[T45] Perl：数组遍历
来源：http://hz.aizwys.cn/gtsfmslpqq.html

for my $x (@arr) { print $x; }
来源：http://hz.ivvv.top/gtbqtmalbt.html

[T46] Perl：哈希操作
来源：http://hz.ydzc1.top/gtxlzhhmqc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.andypj.xyz/gtpqnyfitl.html

[T47] Perl：正则捕获
来源：http://hz.birdmap.top/gtxofqarqr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shuidangran.top/gtxsmpnqqa.html

[T48] Perl：正则替换
来源：http://hz.xinyue.icu/gtdgpngltb.html

$s =~ s/old/new/g;
来源：http://hz.shanyushiyangkeji.top/gtzjfsrigd.html

[T49] Perl：函数
来源：http://hz.zhijiandao.cn/gtmvlsufks.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ywan-chungtsiang.top/gtrodosvfe.html

[T50] Perl：逐行读文件
来源：http://hz.yonumen.top/gtdfocrohl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gzhubu.top/gtydoytqiz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.9152youxi.cn/gticctdvae.html

[T51] Scala：Hello World
来源：http://hz.yuxming.cn/gttluciieu.html

println("Hello")
来源：http://hz.haohaochexian.top/gtjicyglvy.html

[T52] Scala：变量
来源：http://hz.zdqjudy.top/gtmuwlwuwj.html

val a = 1;  var b = 2
来源：http://hz.xuanzx.com/gtumynbryx.html

[T53] Scala：字符串插值
来源：http://hz.jiagoushi.top/gtqnfpghnl.html

s"值: $b"
来源：http://hz.nanxinkj.top/gtxjznwzoc.html

[T54] Scala：集合映射
来源：http://hz.yuanzhike.top/gtwnkmkdbm.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xuanzx.com/gtkhbegtvi.html

[T55] Scala：集合过滤
来源：http://hz.chenlongwang.top/gtllbjdkhx.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydzc1.top/gtjddaodne.html

[T56] Scala：样例类
来源：http://hz.mhx1999.top/gtojyokpke.html

case class User(name: String, age: Int)
来源：http://hz.xylfe.cn/gtkroezzvy.html

[T57] Scala：模式匹配
来源：http://hz.shzxlz.cn/gtixeybnen.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hammf.cn/gtrdwhxxsr.html

[T58] Scala：函数定义
来源：http://hz.yuanzhike.top/gtmrqjhczf.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.meibo888.top/gteanvaoio.html

[T59] Scala：循环
来源：http://hz.chenzaomai.com/gttnomjvtq.html

for (i <- 1 to 10) println(i)
来源：http://hz.yuxming.cn/gtqozkdktm.html

[T60] Scala：折叠
来源：http://hz.havefunace.top/gtvwtcwjvs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shuidangran.top/gteeyethcv.html

================================================================================
来源：http://hz.zhixingplan.top/gtppldcrfx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.daria6918.cn/gtppxqahjs.html

================================================================================
来源：http://hz.9152youxi.cn/gtbfzaxpvt.html

[U01] Py：创建虚拟环境
来源：http://hz.tianlin.xyz/gtuuvucnfv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.dashuyun.cn/gtoeuydhgd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sysykeji.top/gtleuxdnlk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hnxiangtu.top/gtrdikoabd.html

[U03] Py：加载 .env 配置
来源：http://hz.sysykeji.top/gtpgtimata.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jqgfzy.top/gteotxfisu.html

[U04] Py：变量调试打印
来源：http://hz.xylfe.cn/gtlddyyrkn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cqqwz.cn/gtecunqhdd.html

[U05] Py：列表去重且保序
来源：http://hz.yj202588.top/gteqrdogll.html

list(dict.fromkeys(arr))
来源：http://hz.yanxiufei.cn/gtzvxgcwdz.html

[U06] Py：合并两个字典
来源：http://hz.wangdashe.top/gturaydiqu.html

{**a, **b}
来源：http://hz.cheryme.top/gtavchctlk.html

[U07] Py：反转字典键值
来源：http://hz.dashuyun.cn/gtwiyodiid.html

{v: k for k, v in d.items()}
来源：http://hz.aibaodan.cn/gtdjhqiomp.html

[U08] Py：展平二维列表
来源：http://hz.ydjk.org.cn/gtjlgqdldm.html

[y for x in nested for y in x]
来源：http://hz.dashuyun.cn/gtsecgweua.html

[U09] Py：字典取最大值的键
来源：http://hz.yvedp.cn/gtcoabelyi.html

max(d, key=d.get)
来源：http://hz.sysykeji.top/gtwisfltxy.html

[U10] Py：按值排序字典
来源：http://hz.jinqigufen.top/gtzpgnafny.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.fzhhl.top/gtenxiahbq.html

[U11] Py：生成器表达式
来源：http://hz.wangdashe.top/gtgslrffwu.html

(x * 2 for x in arr)
来源：http://hz.52xcode.cn/gtihnnwowr.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cashguo.top/gtfrxowoil.html

Counter(arr).most_common(3)
来源：http://hz.haohaochexian.top/gtljcuybnt.html

[U13] Py：固定长度队列
来源：http://hz.gogol.net.cn/gtwklemhpc.html

deque(maxlen=10)
来源：http://hz.52xcode.cn/gtefdjkbgc.html

[U14] Py：分组收集到列表
来源：http://hz.xingfuxueyuan.xyz/gtqayahavh.html

defaultdict(list)
来源：http://hz.hysaishi.cn/gtnxbnsnef.html

[U15] Py：高精度计时
来源：http://hz.fengsongda.top/gtgvghobck.html

t = time.perf_counter()
来源：http://hz.yj202588.top/gtmhmwfobn.html

[U16] Py：命令行参数解析
来源：http://hz.yueranfly.top/gtssxrwtgs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhaomingkeji.xyz/gtoivurqar.html

[U17] Py：初始化日志
来源：http://hz.jqgfzy.top/gtwydcxzbg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.cheryme.top/gtuazcqvnk.html

[U18] Py：预编译正则
来源：http://hz.pycfn.com/gtnwffeyxj.html

pat = re.compile(r"\d+")
来源：http://hz.hammf.cn/gtukjtvbwh.html

[U19] Py：正则替换带回调
来源：http://hz.yanxiufei.cn/gtegmzpbws.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.andypj.xyz/gtfayqnlkc.html

[U20] Py：缓存函数结果
来源：http://hz.9152youxi.cn/gtmbjmhhzz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shanyushiyangtech.top/gtqskoncml.html

[U21] Py：自定义上下文管理器
来源：http://hz.sysykeji.top/gtkwanvayy.html

@contextlib.contextmanager
来源：http://hz.aizwys.cn/gtwyxuarpg.html

[U22] Py：矩阵转置
来源：http://hz.ywan-chungtsiang.top/gtitiusroy.html

list(zip(*m))
来源：http://hz.zhongyouzk.top/gtdttrtgay.html

[U23] Py：分块读取大文件
来源：http://hz.cashguo.top/gtwpmifypq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cdnleiting.top/gtvigvkcvu.html

[U24] Py：路径操作
来源：http://hz.xuetiantiany.cn/gtyqvhkdwx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.andypj.xyz/gtreewaczf.html

[U25] Py：CSV 按字典读
来源：http://hz.hongshengwenyu.top/gtyyroykqv.html

csv.DictReader(f)
来源：http://hz.hnqzz.top/gterncjmxw.html

[U26] Py：并发下载
来源：http://hz.ivvv.top/gttjdhgyvp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.bjfxy.top/gtggpxvfsw.html

[U27] Py：异步 HTTP
来源：http://hz.hfpthk.cn/gtxunojwwa.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ivvv.top/gteklozpfx.html

[U28] Py：类型别名
来源：http://hz.fengsongda.top/gtjkosusid.html

UserId = int
来源：http://hz.cdnleiting.top/gtezzfuvdr.html

[U29] Py：属性校验
来源：http://hz.hfpthk.cn/gtsdysbmhw.html

@property 与 @x.setter 配合
来源：http://hz.zhoulong.xyz/gtcheopzgp.html

[U30] Py：数据类
来源：http://hz.ywan-chungtsiang.top/gtnstofbds.html

@dataclass(slots=True)
来源：http://hz.xingfuxueyuan.xyz/gtpmypjrfg.html

[U31] Py：单测
来源：http://hz.9152youxi.cn/gtvdgyhaqi.html

python -m pytest -q
来源：http://hz.pycfn.com/gtrpbjrywp.html

[U32] Py：代码格式化
来源：http://hz.xingfuxueyuan.xyz/gtjgoetcdp.html

ruff format . && ruff check --fix .
来源：http://hz.dashuyun.cn/gtapjnutxt.html

[U33] Py：打包发布
来源：http://hz.jinqigfzy.top/gtjjkguytl.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gaohongyu789.top/gtjsfnhhff.html

[U34] Py：判断编码
来源：http://hz.pengpengdd.cyou/gtfeitnyoo.html

chardet.detect(raw)
来源：http://hz.guannengcc.top/gttjxdkcjq.html

[U35] Py：发送邮件
来源：http://hz.shzxlz.cn/gtcseblfxx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cashguo.top/gtbgkzobjw.html

[U36] Py：定时任务
来源：http://hz.hongshengwenyu.top/gtuclprzdk.html

schedule.every(10).minutes.do(job)
来源：http://hz.zdqjudy.top/gtnsyboano.html

[U37] Py：读写 Excel
来源：http://hz.cucudq.cn/gtesqgxgyk.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shanyushiyangtech.top/gtgkenbtue.html

[U38] Py：获取脚本所在目录
来源：http://hz.dashuyun.cn/gtgrqrriee.html

Path(__file__).resolve().parent
来源：http://hz.c1oappe.top/gtigzaujai.html

[U39] Py：判断是否在交互环境
来源：http://hz.wangdashe.top/gtnaksykmv.html

sys.stdout.isatty()
来源：http://hz.hysaishi.cn/gtdmhkixtv.html

[U40] Py：打印到标准错误
来源：http://hz.cashguo.top/gtvgacacbk.html

print("err", file=sys.stderr)
来源：http://hz.hongshengwenyu.top/gteqckcitd.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xylfe.cn/gtcvvrrnjn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yuxming.cn/gtpatsvsxp.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhixingplan.top/gtalgydwfw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.redwolf501.top/gtljsonovb.html

[U43] PHP：声明命名空间
来源：http://hz.guannengcc.top/gtbluxsjns.html

namespace App\Http;
来源：http://hz.gaohongyu789.top/gtjoiisrke.html

[U44] PHP：开启严格类型
来源：http://hz.yueranfly.top/gtmbklotkk.html

declare(strict_types=1);
来源：http://hz.iojbl.cn/gtxwdxgnju.html

[U45] PHP：类型声明与返回类型
来源：http://hz.gzhubu.top/gtkghrclgo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtarkbxvpp.html

[U46] PHP：可空类型
来源：http://hz.ehwqpu.com/gtcwpoudgn.html

?string $name = null
来源：http://hz.zhiwuduotai.top/gtaswtjbwq.html

[U47] PHP：联合类型
来源：http://hz.iojbl.cn/gtwrffiedi.html

int|string $id
来源：http://hz.mhx1999.top/gtapceyvpn.html

[U48] PHP：纯枚举
来源：http://hz.jinyuanbaomall.cn/gtzpbhctvu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.quarkkingdee.top/gtbpnsqluc.html

[U49] PHP：只读属性
来源：http://hz.chenjidiqi.icu/gterqlfzfz.html

public readonly string $name
来源：http://hz.shangyingyoupin.top/gtadstwvlz.html

[U50] PHP：构造器属性提升
来源：http://hz.sweek.top/gtfavzbtop.html

public function __construct(private int $id) {}
来源：http://hz.zycfv.cn/gtwrafllgp.html

[U51] PHP：数组解构
来源：http://hz.shanyushiyangtech.top/gtmkqghgwb.html

[$a, $b] = $arr;
来源：http://hz.gaohongyu789.top/gtcvfoazpm.html

[U52] PHP：箭头函数
来源：http://hz.yonumen.top/gtpaknyuja.html

$double = fn($x) => $x * 2;
来源：http://hz.chenlongwang.top/gtzzccxvqi.html

[U53] PHP：空合并运算符
来源：http://hz.yonumen.top/gtpbcuphsy.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhijiandao.cn/gtvqwkdnvc.html

[U54] PHP：空安全调用
来源：http://hz.zhiwuduotai.top/gtghnbzdmb.html

$obj?->method()
来源：http://hz.tianlin.xyz/gtijawkiaq.html

[U55] PHP：match 表达式
来源：http://hz.xinyue.icu/gtzhmkkkmp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ydzc1.top/gtvmhqtulc.html

[U56] PHP：命名参数
来源：http://hz.jianghu66.top/gthrrlbgdl.html

f(a: 1, b: 2)
来源：http://hz.svipenyu.cn/gtyqeogxdu.html

[U57] PHP：字符串插值
来源：http://hz.havefunace.top/gtritoabcw.html

"值: {$a}"
来源：http://hz.ybcxt.top/gtuzuknjcn.html

[U58] PHP：数组三件套
来源：http://hz.ydjk.org.cn/gtlavinzrk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.bjfxy.top/gtxirqokyr.html

[U59] PHP：自定义排序
来源：http://hz.ehwqpu.com/gtuxtdyidm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aizwys.cn/gtsdtpuwca.html

[U60] PHP：JSON 编解码
来源：http://hz.cqqwz.cn/gtjggmrtqn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ivvv.top/gtprphwnhv.html

[U61] PHP：正则
来源：http://hz.jinyuanbaomall.cn/gtyoeiqgvd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cheryme.top/gtaxqeuxxn.html

[U62] PHP：日期对象
来源：http://hz.hnqzz.top/gtejczggss.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.chenjidiqi.icu/gtbjqhqytw.html

[U63] PHP：文件读写
来源：http://hz.yj20258888.top/gtyjzhcaag.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yanxiufei.cn/gtlzuoqzpz.html

[U64] PHP：目录遍历
来源：http://hz.smart0.xyz/gtwgmweent.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.gotoacloud.top/gtwfykdygf.html

[U65] PHP：会话
来源：http://hz.sweek.top/gtgfrslixt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.wangdashe.top/gtusxbsaps.html

[U66] PHP：设置 Cookie
来源：http://hz.xuetiantiany.cn/gtbcmhsvdz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.nanxinkj.top/gtpljecyiq.html

[U67] PHP：处理文件上传
来源：http://hz.ybcxt.top/gtxuiyswbc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.cashguo.top/gtsfvglrcs.html

[U68] PHP：PDO 连接
来源：http://hz.yongpay.top/gteqbvmceo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hammf.cn/gtcjiozmdy.html

[U69] PHP：PDO 预处理
来源：http://hz.yvedp.cn/gttwpuleub.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jyoumei.cn/gtbdmwjbpa.html

[U70] PHP：PDO 事务
来源：http://hz.daxiang520.top/gtpkbpbggz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.kuanghao11.cn/gtccnlkwwp.html


<!-- 参考信息 -->