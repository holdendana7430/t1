代发 wailian999

while (std::getline(in, line)) { }
来源：http://hz.shuidangran.top/gtgjdzjmbo.html

[S49] C++：写文件
来源：http://hz.shzxlz.cn/gtjzypyslb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenjidiqi.icu/gtolnihoio.html

[S50] C++：格式化数字
来源：http://hz.tian-w.cn/gtbszaeakd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hammf.cn/gtiuroawba.html

[S51] C++：显式类型转换
来源：http://hz.yj202588.top/gtqssijtvi.html

static_cast<double>(a) / b
来源：http://hz.jqgufenzy.top/gtcmblhhwl.html

[S52] C++：const 与 noexcept
来源：http://hz.redwolf501.top/gtptvhwntt.html

int size() const noexcept { return n_; }
来源：http://hz.vqdsnc.cn/gtjxujwjtv.html

[S53] C++：移动语义
来源：http://hz.yuanzhike.top/gtcwfxzmbr.html

std::vector<int> w = std::move(v);
来源：http://hz.cqqwz.cn/gtlfzmrsol.html

[S54] C++：异常处理
来源：http://hz.cheryme.top/gtzapyzwhz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258.top/gtfpsuhkyt.html

[S55] C++：结构化绑定
来源：http://hz.daxiang520.top/gtgpzmjeem.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hnxiangtu.top/gtinayztpv.html

[S56] C++：optional
来源：http://hz.zycfv.cn/gtbkjpoiwn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gogol.net.cn/gtoywxtrbo.html

[S57] C++：编译期常量
来源：http://hz.mhx1999.top/gtpacnbiom.html

constexpr int N = 10;
来源：http://hz.jiagoushi.top/gtfacphrmw.html

[S58] C++：命名空间
来源：http://hz.c1oappe.top/gtsaekuufz.html

namespace ns { int f() { return 1; } }
来源：http://hz.tian-w.cn/gtznnvlmtk.html

[S59] C++：静态断言
来源：http://hz.yueranfly.top/gtxspwlnkz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.smart0.xyz/gtropempzt.html

[S60] C++：遍历并删除元素
来源：http://hz.hywenlv.cn/gtbglstfzb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zdqjudy.top/gtdmsgenqk.html

================================================================================
来源：http://hz.nwbrower.top/gtkofonjfm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ybcxt.top/gtiqvxevky.html

================================================================================
来源：http://hz.jianghu66.top/gthokzcxgh.html

[T01] Kotlin：Hello World
来源：http://hz.nanxinkj.top/gtkzylngtk.html

println("Hello")
来源：http://hz.sysykeji.top/gthkkkktbh.html

[T02] Kotlin：变量
来源：http://hz.ppjwa.cn/gtrgifurfq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jqgfzy.top/gtlermthmp.html

[T03] Kotlin：字符串模板
来源：http://hz.xinyue.icu/gtxambrydj.html

"值: $b"
来源：http://hz.smart0.xyz/gtbzmfkupl.html

[T04] Kotlin：空安全
来源：http://hz.aibaodan.cn/gtlkbwevpk.html

val n: String? = null;  n?.length
来源：http://hz.pycfn.com/gtdsvsbcdv.html

[T05] Kotlin：when 表达式
来源：http://hz.zdqjudy.top/gtouwzxhzu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jlsjyb.cn/gtnotxxcki.html

[T06] Kotlin：集合映射
来源：http://hz.chenzaomai.com/gtlcfqdnrd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.daria6918.cn/gtcgwmowzr.html

[T07] Kotlin：集合过滤
来源：http://hz.haohaochexian.top/gtpdrwxcpu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnqzz.top/gtlafhynrs.html

[T08] Kotlin：数据类
来源：http://hz.yj20258.top/gtbhdtarjl.html

data class User(val name: String, val age: Int)
来源：http://hz.meibo888.top/gtrbxzqiuu.html

[T09] Kotlin：扩展函数
来源：http://hz.jiagoushi.top/gthtmwmhwe.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtnlsvgrgw.html

[T10] Kotlin：默认参数
来源：http://hz.yuxming.cn/gtwspmbkqu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ybcxt.top/gtotnvlgcg.html

[T11] Kotlin：协程
来源：http://hz.tianlin.xyz/gtpbphjdls.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.c1oappe.top/gtywbtsval.html

[T12] Kotlin：解构声明
来源：http://hz.bjfxy.top/gtaxhyoebr.html

val (a, b) = Pair(1, 2)
来源：http://hz.c1oappe.top/gtexpsbfje.html

[T13] Kotlin：只读 Map
来源：http://hz.yanxiufei.cn/gtgystfxzz.html

val m = mapOf("a" to 1)
来源：http://hz.hysaishi.cn/gtzmgjmnav.html

[T14] Kotlin：循环
来源：http://hz.hysaishi.cn/gtllukfctj.html

for (i in 1..10) println(i)
来源：http://hz.zhoulong.xyz/gtyuluihpo.html

[T15] Kotlin：接口
来源：http://hz.cdnleiting.top/gtmfeqhwbi.html

interface Shape { fun area(): Double }
来源：http://hz.redwolf501.top/gtjgvemust.html

[T16] Swift：Hello World
来源：http://hz.mhx1999.top/gtiuelrdmv.html

print("Hello")
来源：http://hz.xinyue.icu/gtzvvyfeko.html

[T17] Swift：变量与常量
来源：http://hz.jinghuilouyu.cn/gtkyyibogn.html

var a = 1;  let b = 2
来源：http://hz.jyoumei.cn/gtndmhlnnf.html

[T18] Swift：字符串插值
来源：http://hz.zhengqikj.top/gtcdavrvhi.html

"值: \(b)"
来源：http://hz.yj20258888.top/gtpmisgttn.html

[T19] Swift：可选绑定
来源：http://hz.yj20258888.top/gttfsfdhoc.html

if let n = opt { print(n) }
来源：http://hz.dianchejie.cn/gtkgecxrmh.html

[T20] Swift：数组操作
来源：http://hz.chenlongwang.top/gtbtxxgado.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fengsongda.top/gteretnssn.html

[T21] Swift：遍历
来源：http://hz.jinghuilouyu.cn/gtlcdcprgg.html

for x in a { print(x) }
来源：http://hz.dianchejie.cn/gtuancqcty.html

[T22] Swift：字典
来源：http://hz.nanxuanxn.top/gtocouvkcv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.0kj1m.cn/gtkjbrwyui.html

[T23] Swift：函数
来源：http://hz.dashuyun.cn/gtermlnkkg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cqqwz.cn/gtlkbpdqsv.html

[T24] Swift：闭包
来源：http://hz.zhaomingkeji.xyz/gtspkwjyjv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinghuilouyu.cn/gtluigcwtj.html

[T25] Swift：结构体
来源：http://hz.jinqigfzy.top/gtvqubqgfo.html

struct P { var x: Int }
来源：http://hz.yj202588.top/gtynrhhrgu.html

[T26] Swift：类与重写
来源：http://hz.gaohongyu789.top/gtbuwbdgpm.html

class A: Base { override func f() {} }
来源：http://hz.snrcjt.cn/gtkxnuufka.html

[T27] Swift：错误处理
来源：http://hz.ppjwa.cn/gttpsxdtqw.html

do { try f() } catch { print(error) }
来源：http://hz.zycfv.cn/gtqlxwasjw.html

[T28] Swift：枚举
来源：http://hz.yj20258888.top/gtotowytxn.html

enum Color { case red, green }
来源：http://hz.gzhubu.top/gtxurrrkar.html

[T29] Swift：guard 提前返回
来源：http://hz.yuxming.cn/gtjkxelkkt.html

guard let x = opt else { return }
来源：http://hz.shanyushiyangkeji.top/gtqdyfpuhd.html

[T30] Swift：协议
来源：http://hz.jqgufenzy.top/gtiwhlnehx.html

protocol Shape { func area() -> Double }
来源：http://hz.svipenyu.cn/gtlzvzathu.html

[T31] Lua：Hello World
来源：http://hz.yvedp.cn/gtkwngboks.html

print("Hello")
来源：http://hz.birdmap.top/gthqdjlczn.html

[T32] Lua：局部变量
来源：http://hz.jinghuilouyu.cn/gttthmmchr.html

local a = 1
来源：http://hz.cheryme.top/gteryxbdml.html

[T33] Lua：表（数组）
来源：http://hz.shuidangran.top/gtljmklsla.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jianghu66.top/gtzvhdtjvv.html

[T34] Lua：遍历表
来源：http://hz.chenjidiqi.icu/gtithnyqnf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.pycfn.com/gtwdvvrtyj.html

[T35] Lua：字典表
来源：http://hz.zhoulong.xyz/gtqdffiznh.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zdqjudy.top/gthmefukkn.html

[T36] Lua：函数
来源：http://hz.jiagoushi.top/gtewikdlhb.html

function add(a, b) return a + b end
来源：http://hz.jianghu66.top/gtpzdhhuxy.html

[T37] Lua：字符串拼接
来源：http://hz.yuanzhike.top/gttckdnrli.html

"a" .. "b"
来源：http://hz.nwbrower.top/gtzmojokcd.html

[T38] Lua：条件
来源：http://hz.yuxming.cn/gtzhzvoigz.html

if x > 0 then print("正") end
来源：http://hz.ybcxt.top/gtesqxaujm.html

[T39] Lua：模式匹配
来源：http://hz.hammf.cn/gtvzzowbqx.html

string.find(s, "%d+")
来源：http://hz.shanyushiyangkeji.top/gttmhyrmzv.html

[T40] Lua：元表
来源：http://hz.vqdsnc.cn/gtikkcoatz.html

setmetatable({}, { __index = base })
来源：http://hz.hnqzz.top/gtzaowxzkl.html

[T41] Perl：Hello World
来源：http://hz.c1oappe.top/gtqsezyanv.html

print "Hello\n";
来源：http://hz.chenlongwang.top/gtbwxfeqsp.html

[T42] Perl：变量类型
来源：http://hz.aizwys.cn/gtzoqwgabp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinyuanbaomall.cn/gtsdlzardn.html

[T43] Perl：字符串插值
来源：http://hz.yj202588.top/gtvkybvifn.html

"值: $a"
来源：http://hz.hywenlv.cn/gtcazpucsh.html

[T44] Perl：条件
来源：http://hz.andypj.xyz/gthoepiond.html

if ($a > 0) { print "正"; }
来源：http://hz.tianlin.xyz/gtrjpjggxw.html

[T45] Perl：数组遍历
来源：http://hz.tanke756.top/gtdenheztt.html

for my $x (@arr) { print $x; }
来源：http://hz.tanke756.top/gtmzxjdrch.html

[T46] Perl：哈希操作
来源：http://hz.yongpay.top/gtqxvsdhgq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.quarkkingdee.top/gtktzrmebg.html

[T47] Perl：正则捕获
来源：http://hz.guowangkeji.top/gtvyurtsyv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xuanzx.com/gtmmbenmfz.html

[T48] Perl：正则替换
来源：http://hz.yonumen.top/gtgzmdfyfx.html

$s =~ s/old/new/g;
来源：http://hz.jiagoushi.top/gtveeagexr.html

[T49] Perl：函数
来源：http://hz.jqgfzy.top/gtvcwojcod.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtqluvqtiv.html

[T50] Perl：逐行读文件
来源：http://hz.mhx1999.top/gtpqtaozyo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhoulong.xyz/gtjollmpfr.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.birdmap.top/gtpfbceslq.html

[T51] Scala：Hello World
来源：http://hz.havefunace.top/gtezcjyhxn.html

println("Hello")
来源：http://hz.dianchejie.cn/gtgbmatitl.html

[T52] Scala：变量
来源：http://hz.jyoumei.cn/gtyanetibr.html

val a = 1;  var b = 2
来源：http://hz.xuetiantiany.cn/gtxzyroppk.html

[T53] Scala：字符串插值
来源：http://hz.ppjwa.cn/gtjtapdbyn.html

s"值: $b"
来源：http://hz.pycfn.com/gtbtiqubse.html

[T54] Scala：集合映射
来源：http://hz.bjfxy.top/gtkhkfytpm.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shanyushiyangkeji.top/gtuyezctvr.html

[T55] Scala：集合过滤
来源：http://hz.nanxinkj.top/gtnnypjycs.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dashuyun.cn/gtmttqasuh.html

[T56] Scala：样例类
来源：http://hz.vqdsnc.cn/gtmebrtibd.html

case class User(name: String, age: Int)
来源：http://hz.yj202588.top/gthuzsrods.html

[T57] Scala：模式匹配
来源：http://hz.shangyingyoupin.top/gtbzcqbgra.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hongshengwenyu.top/gtltcdwbko.html

[T58] Scala：函数定义
来源：http://hz.shuidangran.top/gtqwzzvmhi.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.redwolf501.top/gtybgpblrm.html

[T59] Scala：循环
来源：http://hz.dashuyun.cn/gtkwlrmqmp.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhijiandao.cn/gtzvntheqa.html

[T60] Scala：折叠
来源：http://hz.shanyushiyangkeji.top/gtawsdcvge.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xingfuxueyuan.xyz/gtreaqewki.html

================================================================================
来源：http://hz.xinyue.icu/gtjrdhuybo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydjk.org.cn/gtmvywqxts.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxkyplsrg.html

[U01] Py：创建虚拟环境
来源：http://hz.yj20258888.top/gtfbonhlql.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.pengpengdd.cyou/gtmezrqpfd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sufxvd.cn/gtwpqcpqhs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yueranfly.top/gtisiscpbr.html

[U03] Py：加载 .env 配置
来源：http://hz.jianghu66.top/gtdokgbdbg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.havefunace.top/gttzinjnwk.html

[U04] Py：变量调试打印
来源：http://hz.haohaochexian.top/gtrcgvrsmn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.guannengcc.top/gtvjkntnhp.html

[U05] Py：列表去重且保序
来源：http://hz.yonumen.top/gtrrpawhnt.html

list(dict.fromkeys(arr))
来源：http://hz.chenlongwang.top/gtuvcepzsu.html

[U06] Py：合并两个字典
来源：http://hz.yj202588.top/gtpefwktjv.html

{**a, **b}
来源：http://hz.yj20258.top/gtrarxnzou.html

[U07] Py：反转字典键值
来源：http://hz.52xcode.cn/gtppckbtsj.html

{v: k for k, v in d.items()}
来源：http://hz.havefunace.top/gthqclxbmm.html

[U08] Py：展平二维列表
来源：http://hz.aizwys.cn/gtizdbwenk.html

[y for x in nested for y in x]
来源：http://hz.sysykeji.top/gtebivgxnz.html

[U09] Py：字典取最大值的键
来源：http://hz.daxiang520.top/gtqtsfrhvw.html

max(d, key=d.get)
来源：http://hz.wangshuangyany.cn/gtjbbzzstk.html

[U10] Py：按值排序字典
来源：http://hz.kuanghao11.cn/gtanabpovw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinqigfzy.top/gtslhuvhus.html

[U11] Py：生成器表达式
来源：http://hz.shzxlz.cn/gtbiowsbml.html

(x * 2 for x in arr)
来源：http://hz.hammf.cn/gtrvhropfm.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zdqjudy.top/gtnuemoipn.html

Counter(arr).most_common(3)
来源：http://hz.vqdsnc.cn/gtwskgrnyj.html

[U13] Py：固定长度队列
来源：http://hz.dashuyun.cn/gtdhezbgpl.html

deque(maxlen=10)
来源：http://hz.guannengcc.top/gtgijtmhmv.html

[U14] Py：分组收集到列表
来源：http://hz.cucudq.cn/gtzyoqdcjl.html

defaultdict(list)
来源：http://hz.zhaomingkeji.xyz/gtlrexjsxl.html

[U15] Py：高精度计时
来源：http://hz.zhoulong.xyz/gtmeqloclk.html

t = time.perf_counter()
来源：http://hz.zhongyouzk.top/gtfbrlzwku.html

[U16] Py：命令行参数解析
来源：http://hz.hywenlv.cn/gtqwkgcpxv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.c1oappe.top/gtkuljiwch.html

[U17] Py：初始化日志
来源：http://hz.wangdashe.top/gtzjcoowgy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.52xcode.cn/gtyldcfjcs.html

[U18] Py：预编译正则
来源：http://hz.hfpthk.cn/gthjjodthc.html

pat = re.compile(r"\d+")
来源：http://hz.guannengcc.top/gtljoeojqn.html

[U19] Py：正则替换带回调
来源：http://hz.gogol.net.cn/gtusyjauyj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cheryme.top/gtryibkmts.html

[U20] Py：缓存函数结果
来源：http://hz.yueranfly.top/gtuxrmlbvx.html

@functools.lru_cache(maxsize=None)
来源：http://hz.gogol.net.cn/gtkqvwonwo.html

[U21] Py：自定义上下文管理器
来源：http://hz.ehwqpu.com/gtkldqfnfv.html

@contextlib.contextmanager
来源：http://hz.zycfv.cn/gtbiyzbccd.html

[U22] Py：矩阵转置
来源：http://hz.chenzaomai.com/gtfelqjxpw.html

list(zip(*m))
来源：http://hz.chenlongwang.top/gtwhzbysyr.html

[U23] Py：分块读取大文件
来源：http://hz.gogol.net.cn/gtdaouhibq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ehwqpu.com/gtrigbxkay.html

[U24] Py：路径操作
来源：http://hz.yj20258888.top/gtnwkybjer.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hysaishi.cn/gtxneshhee.html

[U25] Py：CSV 按字典读
来源：http://hz.ivvv.top/gtxuyvtrqy.html

csv.DictReader(f)
来源：http://hz.0kj1m.cn/gtstrintrz.html

[U26] Py：并发下载
来源：http://hz.zhijiandao.cn/gtljjeyjec.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yuxming.cn/gtibwvzlnx.html

[U27] Py：异步 HTTP
来源：http://hz.yonumen.top/gtaxpvrfyd.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.guowangkeji.top/gtucrabjhc.html

[U28] Py：类型别名
来源：http://hz.shzxlz.cn/gtihufqevk.html

UserId = int
来源：http://hz.yj202588.top/gtkzzjdfpz.html

[U29] Py：属性校验
来源：http://hz.hfpthk.cn/gtkvytmkok.html

@property 与 @x.setter 配合
来源：http://hz.andypj.xyz/gtitwgzkdj.html

[U30] Py：数据类
来源：http://hz.kuanghao11.cn/gtlcaverzz.html

@dataclass(slots=True)
来源：http://hz.haohaochexian.top/gtsgudwfzo.html

[U31] Py：单测
来源：http://hz.gaohongyu789.top/gtwggcdbbc.html

python -m pytest -q
来源：http://hz.tianlin.xyz/gtdqmxqzkc.html

[U32] Py：代码格式化
来源：http://hz.zhixingplan.top/gtblsasrgg.html

ruff format . && ruff check --fix .
来源：http://hz.shangyingyoupin.top/gtnkgoifxm.html

[U33] Py：打包发布
来源：http://hz.jiagoushi.top/gttahvihhj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hongshengwenyu.top/gtqawhakiy.html

[U34] Py：判断编码
来源：http://hz.gotoacloud.top/gtfodjcyqo.html

chardet.detect(raw)
来源：http://hz.yuanzhike.top/gtcgqzsrrw.html

[U35] Py：发送邮件
来源：http://hz.nanxuanxn.top/gtdtpkjaqt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.gzhubu.top/gterjfhziu.html

[U36] Py：定时任务
来源：http://hz.hammf.cn/gtfehlrkca.html

schedule.every(10).minutes.do(job)
来源：http://hz.yueranfly.top/gtaqecuarn.html

[U37] Py：读写 Excel
来源：http://hz.pycfn.com/gtihnnaftx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shangyingyoupin.top/gtfgnxulfr.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhoulong.xyz/gtrapkqrzy.html

Path(__file__).resolve().parent
来源：http://hz.ybcxt.top/gtmavxianv.html

[U39] Py：判断是否在交互环境
来源：http://hz.jqgufenzy.top/gtkdlwlhcy.html

sys.stdout.isatty()
来源：http://hz.meibo888.top/gtpxvximdk.html

[U40] Py：打印到标准错误
来源：http://hz.yangfankeji.com/gtfcdaomnr.html

print("err", file=sys.stderr)
来源：http://hz.hnqzz.top/gtqrgekhtt.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sufxvd.cn/gtfcyrgqyp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zycfv.cn/gtlplvpmdz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jinghuilouyu.cn/gtmaeuxnwk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ydjk.org.cn/gtuhwheoqb.html

[U43] PHP：声明命名空间
来源：http://hz.jinghuilouyu.cn/gtswpdeqwd.html

namespace App\Http;
来源：http://hz.nanxuanxn.top/gtjdejmfvs.html

[U44] PHP：开启严格类型
来源：http://hz.jinyuanbaomall.cn/gtdjyaoman.html

declare(strict_types=1);
来源：http://hz.fzhhl.top/gtxpgdzbmz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hnqzz.top/gtcprjqxgl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ybcxt.top/gttekcomut.html

[U46] PHP：可空类型
来源：http://hz.hnxiangtu.top/gtnhckgtda.html

?string $name = null
来源：http://hz.hysaishi.cn/gtrdjqyrtc.html

[U47] PHP：联合类型
来源：http://hz.hammf.cn/gtoicbevue.html

int|string $id
来源：http://hz.gotoacloud.top/gtslmvdfqv.html

[U48] PHP：纯枚举
来源：http://hz.yvedp.cn/gttatdbuxl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.mhx1999.top/gtpwdetqtf.html

[U49] PHP：只读属性
来源：http://hz.hongshengwenyu.top/gthicsrtvd.html

public readonly string $name
来源：http://hz.sufxvd.cn/gtpgiibaxn.html

[U50] PHP：构造器属性提升
来源：http://hz.guowangkeji.top/gtfsoyaocp.html

public function __construct(private int $id) {}
来源：http://hz.nanxuanxn.top/gtuqizrblw.html

[U51] PHP：数组解构
来源：http://hz.gaohongyu789.top/gtbhfodbzm.html

[$a, $b] = $arr;
来源：http://hz.hnqzz.top/gtpjibhszd.html

[U52] PHP：箭头函数
来源：http://hz.yj20258888.top/gtgzryjill.html

$double = fn($x) => $x * 2;
来源：http://hz.vqdsnc.cn/gtqucchjqs.html

[U53] PHP：空合并运算符
来源：http://hz.shuidangran.top/gtukfhpqmh.html

$v = $a ?? $b ?? "default";
来源：http://hz.gzhubu.top/gtgwuheqby.html

[U54] PHP：空安全调用
来源：http://hz.jianghu66.top/gtznhccgxa.html

$obj?->method()
来源：http://hz.cheryme.top/gtbyuwizdl.html

[U55] PHP：match 表达式
来源：http://hz.snrcjt.cn/gtwusqlgeq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.quarkkingdee.top/gtekqacysy.html

[U56] PHP：命名参数
来源：http://hz.daxiang520.top/gtycqzsant.html

f(a: 1, b: 2)
来源：http://hz.tian-w.cn/gttojlfxpw.html

[U57] PHP：字符串插值
来源：http://hz.zhengqikj.top/gteswtfgtw.html

"值: {$a}"
来源：http://hz.dianchejie.cn/gtttveqkrs.html

[U58] PHP：数组三件套
来源：http://hz.birdmap.top/gtvvkxkhnj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ehwqpu.com/gtawwaiqbs.html

[U59] PHP：自定义排序
来源：http://hz.xuanzx.com/gtaubtxpkg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hysaishi.cn/gtcgitnyty.html

[U60] PHP：JSON 编解码
来源：http://hz.yanxiufei.cn/gtagezxxfh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhoulong.xyz/gtguqeorvu.html

[U61] PHP：正则
来源：http://hz.quarkkingdee.top/gtdcppzojv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jyoumei.cn/gtipjrqnel.html

[U62] PHP：日期对象
来源：http://hz.shuidangran.top/gtfydkbrch.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hnqzz.top/gtiicdpaob.html

[U63] PHP：文件读写
来源：http://hz.nanxuanxn.top/gtheiocbim.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhengqikj.top/gtygoyywzk.html

[U64] PHP：目录遍历
来源：http://hz.wangshuangyany.cn/gtmxvpfoeu.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cheryme.top/gtfunynxra.html

[U65] PHP：会话
来源：http://hz.xuanzx.com/gtcvdpmktg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.redwolf501.top/gtqmtzpkbe.html

[U66] PHP：设置 Cookie
来源：http://hz.sufxvd.cn/gtikysihds.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhixingplan.top/gtfpnkznyu.html

[U67] PHP：处理文件上传
来源：http://hz.xylfe.cn/gtylyntaez.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.svipenyu.cn/gtaykryfwi.html

[U68] PHP：PDO 连接
来源：http://hz.wangshuangyany.cn/gtjbctwayy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shanyushiyangkeji.top/gtwmuxobke.html

[U69] PHP：PDO 预处理
来源：http://hz.yanxiufei.cn/gtmhvmiqfd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jinyuanbaomall.cn/gtmazxbmtw.html

[U70] PHP：PDO 事务
来源：http://hz.aizwys.cn/gtaiyvbxtx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.quarkkingdee.top/gtkvrvcryr.html

[U71] PHP：抛出异常
来源：http://hz.xinyue.icu/gtxoswtfcc.html

throw new RuntimeException("失败", 500);
来源：http://hz.fzhhl.top/gtqizzrlxm.html

[U72] PHP：写错误日志
来源：http://hz.bjfxy.top/gtguhbbcmq.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cucudq.cn/gtjdymqnar.html

[U73] PHP：读取 ini 配置
来源：http://hz.ehwqpu.com/gtflldlhbg.html

parse_ini_file("config.ini", true)
来源：http://hz.hnxiangtu.top/gtzgkjxctf.html

[U74] PHP：读取环境变量
来源：http://hz.yueranfly.top/gtpywwfwqj.html

getenv("APP_ENV") ?: "production"
来源：http://hz.ybcxt.top/gtadjhluuj.html


<!-- 参考信息 -->