代发 wailian999

[S45] C++：lambda
来源：http://hz.andypj.xyz/gtljgtgbri.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jqgfzy.top/gtovgxkein.html

[S46] C++：函数模板
来源：http://hz.svipenyu.cn/gtbxrycydx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.andypj.xyz/gtdkfpmobf.html

[S47] C++：结构化绑定遍历
来源：http://hz.sysykeji.top/gthtcndjkx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yuanzhike.top/gtorjfxwis.html

[S48] C++：逐行读文件
来源：http://hz.ydjk.org.cn/gtqmdsupms.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenjidiqi.icu/gtxkgpaulc.html

while (std::getline(in, line)) { }
来源：http://hz.cdnleiting.top/gttupcfspg.html

[S49] C++：写文件
来源：http://hz.shangyingyoupin.top/gtuekzhthw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xingfuxueyuan.xyz/gtxuasgvpp.html

[S50] C++：格式化数字
来源：http://hz.hnxiangtu.top/gtemnkgpoa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ivvv.top/gtkqbphkdv.html

[S51] C++：显式类型转换
来源：http://hz.zdqjudy.top/gtodxwujud.html

static_cast<double>(a) / b
来源：http://hz.zycfv.cn/gtumhnqnvz.html

[S52] C++：const 与 noexcept
来源：http://hz.zhoulong.xyz/gtxvwhnwls.html

int size() const noexcept { return n_; }
来源：http://hz.guannengcc.top/gteonybets.html

[S53] C++：移动语义
来源：http://hz.hysaishi.cn/gtxpnxvinc.html

std::vector<int> w = std::move(v);
来源：http://hz.shuidangran.top/gtjxfjhpwr.html

[S54] C++：异常处理
来源：http://hz.nanxinkj.top/gtscslmvyl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gotoacloud.top/gtwxbgaiyj.html

[S55] C++：结构化绑定
来源：http://hz.zhixingplan.top/gtrpudiabe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhixingplan.top/gtcllcuttu.html

[S56] C++：optional
来源：http://hz.yangfankeji.com/gtxaqnafox.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sufxvd.cn/gtdayuwtvg.html

[S57] C++：编译期常量
来源：http://hz.yj20258.top/gtjuboxtzn.html

constexpr int N = 10;
来源：http://hz.jlsjyb.cn/gtxnhazppy.html

[S58] C++：命名空间
来源：http://hz.shzxlz.cn/gtfflizsni.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgufenzy.top/gtgoaqeypw.html

[S59] C++：静态断言
来源：http://hz.iojbl.cn/gtfatkgngf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sweek.top/gtqvhwiemz.html

[S60] C++：遍历并删除元素
来源：http://hz.snrcjt.cn/gtykueoywa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gogol.net.cn/gthorujyel.html

================================================================================
来源：http://hz.birdmap.top/gtsfixsgow.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgufenzy.top/gtuumnipnn.html

================================================================================
来源：http://hz.yuxming.cn/gtpwvgdzsa.html

[T01] Kotlin：Hello World
来源：http://hz.jlsjyb.cn/gtzikxknth.html

println("Hello")
来源：http://hz.hywenlv.cn/gtlvhzoxgr.html

[T02] Kotlin：变量
来源：http://hz.chenlongwang.top/gttbfxrfgs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.vqdsnc.cn/gtrbubnnkp.html

[T03] Kotlin：字符串模板
来源：http://hz.zhongyouzk.top/gtxrctmcmf.html

"值: $b"
来源：http://hz.hywenlv.cn/gtpydcgotv.html

[T04] Kotlin：空安全
来源：http://hz.nwbrower.top/gtwlaijjil.html

val n: String? = null;  n?.length
来源：http://hz.snrcjt.cn/gtygdyrmjw.html

[T05] Kotlin：when 表达式
来源：http://hz.jinghuilouyu.cn/gteabcfixj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yongpay.top/gtlgfdbvhj.html

[T06] Kotlin：集合映射
来源：http://hz.fengsongda.top/gtvhgnpydm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenzaomai.com/gtwsfhbspg.html

[T07] Kotlin：集合过滤
来源：http://hz.shangyingyoupin.top/gtzhmqwniy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.dianchejie.cn/gtnhfqjsan.html

[T08] Kotlin：数据类
来源：http://hz.gogol.net.cn/gtdtaxpren.html

data class User(val name: String, val age: Int)
来源：http://hz.redwolf501.top/gtkmvsxcgo.html

[T09] Kotlin：扩展函数
来源：http://hz.yj20258.top/gtbalxcvpa.html

fun String.exclaim() = this + "!"
来源：http://hz.yongpay.top/gttbpnbpjq.html

[T10] Kotlin：默认参数
来源：http://hz.zhengqikj.top/gtsxkanapy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xylfe.cn/gtteuswnoj.html

[T11] Kotlin：协程
来源：http://hz.yj202588.top/gthtpvtgpj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.pycfn.com/gtwzhivnyk.html

[T12] Kotlin：解构声明
来源：http://hz.xuetiantiany.cn/gthyznynns.html

val (a, b) = Pair(1, 2)
来源：http://hz.cdnleiting.top/gtuxztdmpt.html

[T13] Kotlin：只读 Map
来源：http://hz.birdmap.top/gtdvdvnuze.html

val m = mapOf("a" to 1)
来源：http://hz.xuanzx.com/gtoqaizvzu.html

[T14] Kotlin：循环
来源：http://hz.0kj1m.cn/gtdrjjpjfv.html

for (i in 1..10) println(i)
来源：http://hz.cqqwz.cn/gttzgcixxr.html

[T15] Kotlin：接口
来源：http://hz.zhixingplan.top/gtzhkjvpcq.html

interface Shape { fun area(): Double }
来源：http://hz.shuidangran.top/gtiptnijxk.html

[T16] Swift：Hello World
来源：http://hz.jiagoushi.top/gtdscapudv.html

print("Hello")
来源：http://hz.jqgfzy.top/gtuymifkkh.html

[T17] Swift：变量与常量
来源：http://hz.xuetiantiany.cn/gtzflvlduz.html

var a = 1;  let b = 2
来源：http://hz.gzhubu.top/gtqimvivrp.html

[T18] Swift：字符串插值
来源：http://hz.yueranfly.top/gtcxjdhxmp.html

"值: \(b)"
来源：http://hz.hysaishi.cn/gtdcoeevqb.html

[T19] Swift：可选绑定
来源：http://hz.havefunace.top/gttngrkmhq.html

if let n = opt { print(n) }
来源：http://hz.wangdashe.top/gtiflusjll.html

[T20] Swift：数组操作
来源：http://hz.jqgufenzy.top/gtmyindqwy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xziqi.cn/gtgpbcucxp.html

[T21] Swift：遍历
来源：http://hz.cheryme.top/gtndfxqfnr.html

for x in a { print(x) }
来源：http://hz.cdnleiting.top/gtgfgbtasj.html

[T22] Swift：字典
来源：http://hz.feifeiyinyue.top/gtvxzkumbr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.andypj.xyz/gttgltotrn.html

[T23] Swift：函数
来源：http://hz.jqgfzy.top/gttmyipawg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ppjwa.cn/gtkwvtmmwq.html

[T24] Swift：闭包
来源：http://hz.kuanghao11.cn/gttxpxkzfy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ppjwa.cn/gtvkiltqqg.html

[T25] Swift：结构体
来源：http://hz.hnxiangtu.top/gtqhkjrgom.html

struct P { var x: Int }
来源：http://hz.shuidangran.top/gtfnxsgnxn.html

[T26] Swift：类与重写
来源：http://hz.birdmap.top/gtcbdpmqup.html

class A: Base { override func f() {} }
来源：http://hz.yuanzhike.top/gtzszpbxet.html

[T27] Swift：错误处理
来源：http://hz.sysykeji.top/gtswyiejas.html

do { try f() } catch { print(error) }
来源：http://hz.zhongyouzk.top/gtadokhnfu.html

[T28] Swift：枚举
来源：http://hz.cashguo.top/gtajqgpebk.html

enum Color { case red, green }
来源：http://hz.gzhubu.top/gttlwrvmxn.html

[T29] Swift：guard 提前返回
来源：http://hz.cashguo.top/gtjrwvrvoq.html

guard let x = opt else { return }
来源：http://hz.zhoulong.xyz/gtkfaoaqsm.html

[T30] Swift：协议
来源：http://hz.9152youxi.cn/gtpiftfcxi.html

protocol Shape { func area() -> Double }
来源：http://hz.ywan-chungtsiang.top/gtbsimdluk.html

[T31] Lua：Hello World
来源：http://hz.feifeiyinyue.top/gtehfnhsjh.html

print("Hello")
来源：http://hz.ehwqpu.com/gtslpojofk.html

[T32] Lua：局部变量
来源：http://hz.zhiwuduotai.top/gtkyrsduwr.html

local a = 1
来源：http://hz.zdqjudy.top/gtbtizqtdm.html

[T33] Lua：表（数组）
来源：http://hz.yj20258.top/gtltszptai.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gotoacloud.top/gtyhvotmhp.html

[T34] Lua：遍历表
来源：http://hz.tianlin.xyz/gtrkxawdvm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.c1oappe.top/gttpqxtlrk.html

[T35] Lua：字典表
来源：http://hz.zhoulong.xyz/gtfxzgtxsi.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinyuanbaomall.cn/gtjnybyieb.html

[T36] Lua：函数
来源：http://hz.cucudq.cn/gtmdqkzdko.html

function add(a, b) return a + b end
来源：http://hz.xziqi.cn/gtkzgkjyfz.html

[T37] Lua：字符串拼接
来源：http://hz.yonumen.top/gtuekpkury.html

"a" .. "b"
来源：http://hz.yangfankeji.com/gtzttrvwbc.html

[T38] Lua：条件
来源：http://hz.shanyushiyangkeji.top/gtotjyfqfb.html

if x > 0 then print("正") end
来源：http://hz.shanyushiyangtech.top/gtcnqaisrd.html

[T39] Lua：模式匹配
来源：http://hz.zhaomingkeji.xyz/gthzexadse.html

string.find(s, "%d+")
来源：http://hz.dianchejie.cn/gtplljvqyw.html

[T40] Lua：元表
来源：http://hz.guannengcc.top/gtbwuqbbik.html

setmetatable({}, { __index = base })
来源：http://hz.yj20258.top/gtpxeyrlcu.html

[T41] Perl：Hello World
来源：http://hz.shuidangran.top/gtldpwuclr.html

print "Hello\n";
来源：http://hz.sxryk.cn/gtsmrmvtnp.html

[T42] Perl：变量类型
来源：http://hz.c1oappe.top/gtcoxjtdze.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.guowangkeji.top/gtolfsjqtw.html

[T43] Perl：字符串插值
来源：http://hz.tanke756.top/gtnsurxbuc.html

"值: $a"
来源：http://hz.shanyushiyangtech.top/gtwjpgmfdw.html

[T44] Perl：条件
来源：http://hz.hfpthk.cn/gtcalgmgum.html

if ($a > 0) { print "正"; }
来源：http://hz.kuanghao11.cn/gtohmncnlm.html

[T45] Perl：数组遍历
来源：http://hz.pycfn.com/gtxqlrxjqg.html

for my $x (@arr) { print $x; }
来源：http://hz.pycfn.com/gtaaiucoaf.html

[T46] Perl：哈希操作
来源：http://hz.kuanghao11.cn/gttzdesilk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.feifeiyinyue.top/gtrudnuqmx.html

[T47] Perl：正则捕获
来源：http://hz.tanke756.top/gtilpiepft.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.pycfn.com/gtpumrubwg.html

[T48] Perl：正则替换
来源：http://hz.yj20258888.top/gtbbxhywqt.html

$s =~ s/old/new/g;
来源：http://hz.ivvv.top/gtjkktcecs.html

[T49] Perl：函数
来源：http://hz.yueranfly.top/gtgoxrzgwf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.fzhhl.top/gtukhhmnth.html

[T50] Perl：逐行读文件
来源：http://hz.wangshuangyany.cn/gtbrdflsql.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jqgufenzy.top/gtspuvqiqh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.9152youxi.cn/gtdoquvdst.html

[T51] Scala：Hello World
来源：http://hz.yuxming.cn/gttpgsjrbc.html

println("Hello")
来源：http://hz.sxryk.cn/gtmceteisv.html

[T52] Scala：变量
来源：http://hz.pengpengdd.cyou/gtvvztjrdt.html

val a = 1;  var b = 2
来源：http://hz.shanyushiyangtech.top/gtvcwxlfhx.html

[T53] Scala：字符串插值
来源：http://hz.zhoulong.xyz/gtaacwnhie.html

s"值: $b"
来源：http://hz.cashguo.top/gtentdzqdr.html

[T54] Scala：集合映射
来源：http://hz.yuanzhike.top/gthsfhtccz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yvedp.cn/gtnwatugkt.html

[T55] Scala：集合过滤
来源：http://hz.daria6918.cn/gtfwozztfm.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jqgufenzy.top/gtmqaodcfc.html

[T56] Scala：样例类
来源：http://hz.feifeiyinyue.top/gtjfowvzny.html

case class User(name: String, age: Int)
来源：http://hz.yvedp.cn/gtwfxvpdxq.html

[T57] Scala：模式匹配
来源：http://hz.yj20258888.top/gtzggzlzff.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.kuanghao11.cn/gtzavtsdmo.html

[T58] Scala：函数定义
来源：http://hz.ppjwa.cn/gtcsdvhwbz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hnxiangtu.top/gtmtdhmedl.html

[T59] Scala：循环
来源：http://hz.daxiang520.top/gtnbexyysm.html

for (i <- 1 to 10) println(i)
来源：http://hz.smart0.xyz/gtnsauboya.html

[T60] Scala：折叠
来源：http://hz.nanxuanxn.top/gtswynmkpw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yuxming.cn/gtejxabjyh.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtepjqxblx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shuidangran.top/gtyltqxboi.html

================================================================================
来源：http://hz.yonumen.top/gtcqhpomuo.html

[U01] Py：创建虚拟环境
来源：http://hz.andypj.xyz/gttpmtsgdb.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.52xcode.cn/gtnceqgmkb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zdqjudy.top/gtwqmjnzzt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xuanzx.com/gtebqslhqe.html

[U03] Py：加载 .env 配置
来源：http://hz.jiagoushi.top/gtyqsjcsks.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.nwbrower.top/gtirgnuoge.html

[U04] Py：变量调试打印
来源：http://hz.zhixingplan.top/gtkmjyetqx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhengqikj.top/gtfydbmljk.html

[U05] Py：列表去重且保序
来源：http://hz.sufxvd.cn/gtzxbskhkv.html

list(dict.fromkeys(arr))
来源：http://hz.cheryme.top/gthcgjpwri.html

[U06] Py：合并两个字典
来源：http://hz.shzxlz.cn/gtynzbpqet.html

{**a, **b}
来源：http://hz.guowangkeji.top/gtckwgugjy.html

[U07] Py：反转字典键值
来源：http://hz.yj20258888.top/gtftbdpbvg.html

{v: k for k, v in d.items()}
来源：http://hz.jyoumei.cn/gtrggesdfx.html

[U08] Py：展平二维列表
来源：http://hz.jyoumei.cn/gtofncywgm.html

[y for x in nested for y in x]
来源：http://hz.nanxuanxn.top/gtlmpguhgk.html

[U09] Py：字典取最大值的键
来源：http://hz.shanyushiyangtech.top/gtgutbuhrp.html

max(d, key=d.get)
来源：http://hz.52xcode.cn/gtgzusxqtw.html

[U10] Py：按值排序字典
来源：http://hz.gogol.net.cn/gtdlksyvuv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinqigufen.top/gtyfnwiofl.html

[U11] Py：生成器表达式
来源：http://hz.chenlongwang.top/gtpvoaldwp.html

(x * 2 for x in arr)
来源：http://hz.cashguo.top/gtdwkvtjic.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ppjwa.cn/gtmgblaidk.html

Counter(arr).most_common(3)
来源：http://hz.feifeiyinyue.top/gtbcldtutf.html

[U13] Py：固定长度队列
来源：http://hz.tian-w.cn/gtqkkyiceu.html

deque(maxlen=10)
来源：http://hz.0kj1m.cn/gtlfqxmnrd.html

[U14] Py：分组收集到列表
来源：http://hz.jinyuanbaomall.cn/gtwnguwmsu.html

defaultdict(list)
来源：http://hz.zdqjudy.top/gtnwcrhhbz.html

[U15] Py：高精度计时
来源：http://hz.cheryme.top/gtsxbyhvgd.html

t = time.perf_counter()
来源：http://hz.9152youxi.cn/gtdnptlrxj.html

[U16] Py：命令行参数解析
来源：http://hz.guowangkeji.top/gtzcmwvrhx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.tianlin.xyz/gtiwaneyps.html

[U17] Py：初始化日志
来源：http://hz.hnqzz.top/gtppdlhrad.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.aibaodan.cn/gtedlscacj.html

[U18] Py：预编译正则
来源：http://hz.316326.xyz/gtusdimrzm.html

pat = re.compile(r"\d+")
来源：http://hz.chenjidiqi.icu/gtimeyscnn.html

[U19] Py：正则替换带回调
来源：http://hz.tianlin.xyz/gtorxpsstu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hywenlv.cn/gtrjoqnaiq.html

[U20] Py：缓存函数结果
来源：http://hz.ehwqpu.com/gtdycjycgt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.havefunace.top/gtwphcrhim.html

[U21] Py：自定义上下文管理器
来源：http://hz.smart0.xyz/gtpnyignxy.html

@contextlib.contextmanager
来源：http://hz.cheryme.top/gtnzevyhaw.html

[U22] Py：矩阵转置
来源：http://hz.ywan-chungtsiang.top/gtxguulvko.html

list(zip(*m))
来源：http://hz.birdmap.top/gtrntzcoxw.html

[U23] Py：分块读取大文件
来源：http://hz.cheryme.top/gtozxiirfj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jlsjyb.cn/gthlrshkyl.html

[U24] Py：路径操作
来源：http://hz.redwolf501.top/gtmnmbxrrf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinghuilouyu.cn/gtkvishgvz.html

[U25] Py：CSV 按字典读
来源：http://hz.jinyuanbaomall.cn/gtzogexbpg.html

csv.DictReader(f)
来源：http://hz.hfpthk.cn/gtzavybnvu.html

[U26] Py：并发下载
来源：http://hz.zhijiandao.cn/gtonngrhbo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xuetiantiany.cn/gtgcuwlogq.html

[U27] Py：异步 HTTP
来源：http://hz.svipenyu.cn/gtcjtywbek.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.pengpengdd.cyou/gtrtcszeut.html

[U28] Py：类型别名
来源：http://hz.316326.xyz/gtmbiulztn.html

UserId = int
来源：http://hz.jianghu66.top/gthknmgyqm.html

[U29] Py：属性校验
来源：http://hz.sweek.top/gtxpdrxhbj.html

@property 与 @x.setter 配合
来源：http://hz.guannengcc.top/gtjhgdxchr.html

[U30] Py：数据类
来源：http://hz.wangdashe.top/gtdrxetoty.html

@dataclass(slots=True)
来源：http://hz.ivvv.top/gtimtpncwk.html

[U31] Py：单测
来源：http://hz.ehwqpu.com/gtkuoxmdnp.html

python -m pytest -q
来源：http://hz.yanxiufei.cn/gtbutbjxif.html

[U32] Py：代码格式化
来源：http://hz.sysykeji.top/gtseihhtmm.html

ruff format . && ruff check --fix .
来源：http://hz.xingfuxueyuan.xyz/gtlwwptnae.html

[U33] Py：打包发布
来源：http://hz.shanyushiyangkeji.top/gtfoauppjs.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.birdmap.top/gtejsgvygl.html

[U34] Py：判断编码
来源：http://hz.dashuyun.cn/gthlgbumws.html

chardet.detect(raw)
来源：http://hz.zhiwuduotai.top/gttjmdyiye.html

[U35] Py：发送邮件
来源：http://hz.zhoulong.xyz/gtmigzofyn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.wangshuangyany.cn/gtsbysfdgm.html

[U36] Py：定时任务
来源：http://hz.zhaomingkeji.xyz/gtzkngavwi.html

schedule.every(10).minutes.do(job)
来源：http://hz.birdmap.top/gtdtyklwho.html

[U37] Py：读写 Excel
来源：http://hz.c1oappe.top/gtoeyhogbq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhengqikj.top/gtebvveiol.html

[U38] Py：获取脚本所在目录
来源：http://hz.c1oappe.top/gtytlcwamj.html

Path(__file__).resolve().parent
来源：http://hz.fzhhl.top/gtlyuasicf.html

[U39] Py：判断是否在交互环境
来源：http://hz.xuetiantiany.cn/gtdjbgfylu.html

sys.stdout.isatty()
来源：http://hz.daria6918.cn/gtpvgbiyjj.html

[U40] Py：打印到标准错误
来源：http://hz.yanxiufei.cn/gtryfhkoev.html

print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtddjcvycu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.aizwys.cn/gtyhltrlwd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.gzhubu.top/gtzpgveqmy.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xziqi.cn/gtrmgrtgqc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jyoumei.cn/gtrbnvazjl.html

[U43] PHP：声明命名空间
来源：http://hz.zhiwuduotai.top/gtivybysfe.html

namespace App\Http;
来源：http://hz.andypj.xyz/gtrzstmnur.html

[U44] PHP：开启严格类型
来源：http://hz.zhixingplan.top/gtinuqsuqu.html

declare(strict_types=1);
来源：http://hz.hammf.cn/gtvyfcqokw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cheryme.top/gtpqdzqyin.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigfzy.top/gtfcrqfqdj.html

[U46] PHP：可空类型
来源：http://hz.andypj.xyz/gtztqpyrxx.html

?string $name = null
来源：http://hz.yueranfly.top/gtkvpxjoxy.html

[U47] PHP：联合类型
来源：http://hz.sysykeji.top/gtjujynevw.html

int|string $id
来源：http://hz.yuxming.cn/gtohzsjjzm.html

[U48] PHP：纯枚举
来源：http://hz.yuanzhike.top/gtevqrwduz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ehwqpu.com/gtaclryyob.html

[U49] PHP：只读属性
来源：http://hz.hongshengwenyu.top/gtbsckkjfo.html

public readonly string $name
来源：http://hz.chenlongwang.top/gtawtjbzrl.html

[U50] PHP：构造器属性提升
来源：http://hz.ppjwa.cn/gtlanzxkef.html

public function __construct(private int $id) {}
来源：http://hz.feifeiyinyue.top/gtclkanntv.html

[U51] PHP：数组解构
来源：http://hz.cashguo.top/gtphcvquew.html

[$a, $b] = $arr;
来源：http://hz.feifeiyinyue.top/gtbzqvyhta.html

[U52] PHP：箭头函数
来源：http://hz.jiagoushi.top/gthykhlphr.html

$double = fn($x) => $x * 2;
来源：http://hz.yangfankeji.com/gtgdnaezci.html

[U53] PHP：空合并运算符
来源：http://hz.xylfe.cn/gtvbdyumvb.html

$v = $a ?? $b ?? "default";
来源：http://hz.c1oappe.top/gtjxrsdphy.html

[U54] PHP：空安全调用
来源：http://hz.gaohongyu789.top/gtchrfofbh.html

$obj?->method()
来源：http://hz.cdnleiting.top/gtcxgxwgtr.html

[U55] PHP：match 表达式
来源：http://hz.gzhubu.top/gtrfcnlrwn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.andypj.xyz/gtdnslituk.html

[U56] PHP：命名参数
来源：http://hz.yonumen.top/gtlwgcsycw.html

f(a: 1, b: 2)
来源：http://hz.hfpthk.cn/gtqevuvylj.html

[U57] PHP：字符串插值
来源：http://hz.yangfankeji.com/gtdgjsrdsu.html

"值: {$a}"
来源：http://hz.yuanzhike.top/gteatxtrzf.html

[U58] PHP：数组三件套
来源：http://hz.zhengqikj.top/gtmpamzlyz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.gotoacloud.top/gtimfakcll.html

[U59] PHP：自定义排序
来源：http://hz.hnxiangtu.top/gtikyskjwx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xinyue.icu/gtjmuvsrhb.html

[U60] PHP：JSON 编解码
来源：http://hz.guowangkeji.top/gtysjarjgm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.fengsongda.top/gtvzfaeozj.html

[U61] PHP：正则
来源：http://hz.gaohongyu789.top/gtaldirrkt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.tianlin.xyz/gtbygzswjv.html

[U62] PHP：日期对象
来源：http://hz.xinyue.icu/gtfalnohpz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.aizwys.cn/gtlclhmjpj.html

[U63] PHP：文件读写
来源：http://hz.52xcode.cn/gtturwgaxg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj20258.top/gtxgdraqen.html

[U64] PHP：目录遍历
来源：http://hz.yueranfly.top/gtdjxjawdo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cashguo.top/gttmtdkvbl.html

[U65] PHP：会话
来源：http://hz.jinqigfzy.top/gttwlkxmzx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.guannengcc.top/gtzyozzaad.html

[U66] PHP：设置 Cookie
来源：http://hz.chenjidiqi.icu/gthyndedua.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.fengsongda.top/gtmqtrwptn.html

[U67] PHP：处理文件上传
来源：http://hz.yj202588.top/gtlcvwqhjd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.chenlongwang.top/gtsmmvclgm.html

[U68] PHP：PDO 连接
来源：http://hz.gotoacloud.top/gtpdocugsw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jinyuanbaomall.cn/gtgftikqix.html

[U69] PHP：PDO 预处理
来源：http://hz.ivvv.top/gtrgxmfoae.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cucudq.cn/gtqlkfbtkt.html

[U70] PHP：PDO 事务
来源：http://hz.svipenyu.cn/gtbwkgjwew.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xuetiantiany.cn/gtmhswgwms.html


<!-- 参考信息 -->