代发 wailian999

[S45] C++：lambda
来源：http://hz.nwbrower.top/gtepzrqbue.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.vqdsnc.cn/gtxellmhuz.html

[S46] C++：函数模板
来源：http://hz.jlsjyb.cn/gtccysrwpw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sxryk.cn/gtrehjxhvz.html

[S47] C++：结构化绑定遍历
来源：http://hz.xylfe.cn/gtvsfyfaox.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ppjwa.cn/gtbuclmfgj.html

[S48] C++：逐行读文件
来源：http://hz.9152youxi.cn/gtveoinqfb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ivvv.top/gtlltcexhj.html

while (std::getline(in, line)) { }
来源：http://hz.aizwys.cn/gtfsdczace.html

[S49] C++：写文件
来源：http://hz.vqdsnc.cn/gtxtelntao.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cdnleiting.top/gtlngomezb.html

[S50] C++：格式化数字
来源：http://hz.aizwys.cn/gtodfqgogz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hammf.cn/gtaddkdetk.html

[S51] C++：显式类型转换
来源：http://hz.jqgufenzy.top/gtjkjeczbw.html

static_cast<double>(a) / b
来源：http://hz.ivvv.top/gthjsejmqv.html

[S52] C++：const 与 noexcept
来源：http://hz.316326.xyz/gtvopwilwa.html

int size() const noexcept { return n_; }
来源：http://hz.yonumen.top/gtehliimlg.html

[S53] C++：移动语义
来源：http://hz.wangshuangyany.cn/gtnqrajfdx.html

std::vector<int> w = std::move(v);
来源：http://hz.dianchejie.cn/gtnqcmhacc.html

[S54] C++：异常处理
来源：http://hz.jianghu66.top/gtxlgqmcgv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ppjwa.cn/gtddojxalk.html

[S55] C++：结构化绑定
来源：http://hz.yanxiufei.cn/gtjoyntglm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tianlin.xyz/gtxlnisgyg.html

[S56] C++：optional
来源：http://hz.cucudq.cn/gtqpxrdhhf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gogol.net.cn/gtuskjfehf.html

[S57] C++：编译期常量
来源：http://hz.nwbrower.top/gtnmrptojv.html

constexpr int N = 10;
来源：http://hz.gzhubu.top/gtdftqnyab.html

[S58] C++：命名空间
来源：http://hz.snrcjt.cn/gtuiutvvvq.html

namespace ns { int f() { return 1; } }
来源：http://hz.yongpay.top/gttuunjfet.html

[S59] C++：静态断言
来源：http://hz.zhengqikj.top/gtqoxwkziv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ywan-chungtsiang.top/gtgkdwonxl.html

[S60] C++：遍历并删除元素
来源：http://hz.c1oappe.top/gtgdewfwjl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gogol.net.cn/gtbrsmjtwo.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtkmahkejh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.meibo888.top/gtvjroavoo.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxiidxbqh.html

[T01] Kotlin：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtsqnbmfwj.html

println("Hello")
来源：http://hz.hnxiangtu.top/gthmnrovyn.html

[T02] Kotlin：变量
来源：http://hz.hammf.cn/gttgwsllkb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gotoacloud.top/gtxgwrlhnq.html

[T03] Kotlin：字符串模板
来源：http://hz.zhijiandao.cn/gtmdclwyrl.html

"值: $b"
来源：http://hz.haohaochexian.top/gtbsosxqkl.html

[T04] Kotlin：空安全
来源：http://hz.hfpthk.cn/gtwmflwsqq.html

val n: String? = null;  n?.length
来源：http://hz.fzhhl.top/gttbatliwl.html

[T05] Kotlin：when 表达式
来源：http://hz.cqqwz.cn/gtftxrhhjb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yonumen.top/gtravsfwcz.html

[T06] Kotlin：集合映射
来源：http://hz.jlsjyb.cn/gtsyfgnkep.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shzxlz.cn/gthbtwhazi.html

[T07] Kotlin：集合过滤
来源：http://hz.sweek.top/gtdgaxlnkk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.haohaochexian.top/gtkzyxrhxs.html

[T08] Kotlin：数据类
来源：http://hz.cqqwz.cn/gtdsaqknif.html

data class User(val name: String, val age: Int)
来源：http://hz.zhaomingkeji.xyz/gtledqtqcq.html

[T09] Kotlin：扩展函数
来源：http://hz.shuidangran.top/gtvgfpurvf.html

fun String.exclaim() = this + "!"
来源：http://hz.jlsjyb.cn/gtglqftxjm.html

[T10] Kotlin：默认参数
来源：http://hz.dianchejie.cn/gtfeeoyysz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.andypj.xyz/gtvmzhsaad.html

[T11] Kotlin：协程
来源：http://hz.jianghu66.top/gtfwnixseg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhongyouzk.top/gttcprmlgm.html

[T12] Kotlin：解构声明
来源：http://hz.xingfuxueyuan.xyz/gtksixtisx.html

val (a, b) = Pair(1, 2)
来源：http://hz.316326.xyz/gtaofsvjwx.html

[T13] Kotlin：只读 Map
来源：http://hz.feifeiyinyue.top/gtkndmzwsf.html

val m = mapOf("a" to 1)
来源：http://hz.52xcode.cn/gtegqfvotp.html

[T14] Kotlin：循环
来源：http://hz.gotoacloud.top/gtqabydnoy.html

for (i in 1..10) println(i)
来源：http://hz.cqqwz.cn/gtfrmvivbp.html

[T15] Kotlin：接口
来源：http://hz.nanxuanxn.top/gttfaqxjeb.html

interface Shape { fun area(): Double }
来源：http://hz.jiagoushi.top/gtbctfkudu.html

[T16] Swift：Hello World
来源：http://hz.ybcxt.top/gtvkcmcklb.html

print("Hello")
来源：http://hz.hfpthk.cn/gtgremjssn.html

[T17] Swift：变量与常量
来源：http://hz.sxryk.cn/gtyscwwvlc.html

var a = 1;  let b = 2
来源：http://hz.xuetiantiany.cn/gtwagyzjdz.html

[T18] Swift：字符串插值
来源：http://hz.hnqzz.top/gtmgdmeror.html

"值: \(b)"
来源：http://hz.aizwys.cn/gteyfwcbjh.html

[T19] Swift：可选绑定
来源：http://hz.52xcode.cn/gtklmjbgof.html

if let n = opt { print(n) }
来源：http://hz.andypj.xyz/gtfczvmprd.html

[T20] Swift：数组操作
来源：http://hz.yueranfly.top/gthwfriyro.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gogol.net.cn/gtdsmznmvq.html

[T21] Swift：遍历
来源：http://hz.yanxiufei.cn/gtgibtnugz.html

for x in a { print(x) }
来源：http://hz.shzxlz.cn/gtlbpresui.html

[T22] Swift：字典
来源：http://hz.yvedp.cn/gtdxymmfwx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xinyue.icu/gtrfpkxkyf.html

[T23] Swift：函数
来源：http://hz.xinyue.icu/gthyerkoxy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jlsjyb.cn/gtceagnoes.html

[T24] Swift：闭包
来源：http://hz.zycfv.cn/gtbkcqdzse.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ivvv.top/gtlanwicvm.html

[T25] Swift：结构体
来源：http://hz.yonumen.top/gtnwurhovd.html

struct P { var x: Int }
来源：http://hz.chenjidiqi.icu/gtykbrdekq.html

[T26] Swift：类与重写
来源：http://hz.jyoumei.cn/gtkcuuwyon.html

class A: Base { override func f() {} }
来源：http://hz.chenzaomai.com/gtodbcxrlu.html

[T27] Swift：错误处理
来源：http://hz.smart0.xyz/gtpesfcuol.html

do { try f() } catch { print(error) }
来源：http://hz.jinghuilouyu.cn/gtkvygculb.html

[T28] Swift：枚举
来源：http://hz.nanxinkj.top/gtxssulnae.html

enum Color { case red, green }
来源：http://hz.gzhubu.top/gtullzzkse.html

[T29] Swift：guard 提前返回
来源：http://hz.yueranfly.top/gtarmtbees.html

guard let x = opt else { return }
来源：http://hz.chenlongwang.top/gtuaqleobd.html

[T30] Swift：协议
来源：http://hz.cheryme.top/gtdbcfcqoy.html

protocol Shape { func area() -> Double }
来源：http://hz.cashguo.top/gtekszmnoa.html

[T31] Lua：Hello World
来源：http://hz.vqdsnc.cn/gtukgzspab.html

print("Hello")
来源：http://hz.meibo888.top/gtcronnbyk.html

[T32] Lua：局部变量
来源：http://hz.sxryk.cn/gtnaoxtfvm.html

local a = 1
来源：http://hz.zhongyouzk.top/gtswfbvzft.html

[T33] Lua：表（数组）
来源：http://hz.9152youxi.cn/gtclhwbzvy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhijiandao.cn/gtcsabfrpk.html

[T34] Lua：遍历表
来源：http://hz.shuidangran.top/gtjgyanoxp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ehwqpu.com/gtzxivqzia.html

[T35] Lua：字典表
来源：http://hz.zycfv.cn/gthmaxbehb.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinyuanbaomall.cn/gtzbnlmcaz.html

[T36] Lua：函数
来源：http://hz.ivvv.top/gtxfhkdovo.html

function add(a, b) return a + b end
来源：http://hz.daria6918.cn/gtoysntfuk.html

[T37] Lua：字符串拼接
来源：http://hz.xylfe.cn/gtfhboaivs.html

"a" .. "b"
来源：http://hz.cashguo.top/gtbavriuaa.html

[T38] Lua：条件
来源：http://hz.cucudq.cn/gtmzgnscqy.html

if x > 0 then print("正") end
来源：http://hz.jinqigfzy.top/gtwmtsybmh.html

[T39] Lua：模式匹配
来源：http://hz.kuanghao11.cn/gtlhtlvegg.html

string.find(s, "%d+")
来源：http://hz.gotoacloud.top/gtahmpngny.html

[T40] Lua：元表
来源：http://hz.fzhhl.top/gtnkernijr.html

setmetatable({}, { __index = base })
来源：http://hz.mhx1999.top/gtkohhwdlb.html

[T41] Perl：Hello World
来源：http://hz.zhaomingkeji.xyz/gtguiftlqk.html

print "Hello\n";
来源：http://hz.kuanghao11.cn/gtawznsgmn.html

[T42] Perl：变量类型
来源：http://hz.chenzaomai.com/gtdxqygnos.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yueranfly.top/gtlxamqswk.html

[T43] Perl：字符串插值
来源：http://hz.shanyushiyangtech.top/gtloubixot.html

"值: $a"
来源：http://hz.yongpay.top/gtluefhbaq.html

[T44] Perl：条件
来源：http://hz.andypj.xyz/gtjvttdkne.html

if ($a > 0) { print "正"; }
来源：http://hz.pycfn.com/gtqobnsueu.html

[T45] Perl：数组遍历
来源：http://hz.cqqwz.cn/gtwqexhsku.html

for my $x (@arr) { print $x; }
来源：http://hz.havefunace.top/gtdffvmbwb.html

[T46] Perl：哈希操作
来源：http://hz.dashuyun.cn/gtugbekglf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xziqi.cn/gtqnwigrln.html

[T47] Perl：正则捕获
来源：http://hz.sysykeji.top/gtohxypbmm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xinyue.icu/gtbuvckxmp.html

[T48] Perl：正则替换
来源：http://hz.xziqi.cn/gtpbymxysz.html

$s =~ s/old/new/g;
来源：http://hz.jiagoushi.top/gtuciklxyq.html

[T49] Perl：函数
来源：http://hz.quarkkingdee.top/gtwdjdsdnj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gotoacloud.top/gtzigtmuuc.html

[T50] Perl：逐行读文件
来源：http://hz.zycfv.cn/gtqysacdoj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.havefunace.top/gtchtoymyb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.snrcjt.cn/gthjopniie.html

[T51] Scala：Hello World
来源：http://hz.yueranfly.top/gtwulubwmn.html

println("Hello")
来源：http://hz.meibo888.top/gtwnelnstn.html

[T52] Scala：变量
来源：http://hz.gotoacloud.top/gtewhswljk.html

val a = 1;  var b = 2
来源：http://hz.hfpthk.cn/gtbigqdxbq.html

[T53] Scala：字符串插值
来源：http://hz.jlsjyb.cn/gtxrerjlls.html

s"值: $b"
来源：http://hz.hammf.cn/gtsarntxyw.html

[T54] Scala：集合映射
来源：http://hz.wangshuangyany.cn/gtbtwaxejr.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.tanke756.top/gtukhvxkst.html

[T55] Scala：集合过滤
来源：http://hz.yj20258.top/gtcxrrpjjy.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hnqzz.top/gtxgaabarr.html

[T56] Scala：样例类
来源：http://hz.redwolf501.top/gtgxbnkkcb.html

case class User(name: String, age: Int)
来源：http://hz.chenzaomai.com/gtxejeoqrt.html

[T57] Scala：模式匹配
来源：http://hz.gzhubu.top/gtejbzjrvn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.316326.xyz/gtxiezsjha.html

[T58] Scala：函数定义
来源：http://hz.zhengqikj.top/gtlynmdtxo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ywan-chungtsiang.top/gtaohpfsli.html

[T59] Scala：循环
来源：http://hz.wangshuangyany.cn/gtifbqzosb.html

for (i <- 1 to 10) println(i)
来源：http://hz.wangdashe.top/gtdgjpbtcp.html

[T60] Scala：折叠
来源：http://hz.0kj1m.cn/gtkrcrtekj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shanyushiyangtech.top/gtznihllsn.html

================================================================================
来源：http://hz.fengsongda.top/gtqerapfbk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhiwuduotai.top/gtsszxukjo.html

================================================================================
来源：http://hz.iojbl.cn/gtfzlffgxv.html

[U01] Py：创建虚拟环境
来源：http://hz.pycfn.com/gtoiuzfypd.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yangfankeji.com/gtruzzrump.html

[U02] Py：导出 / 安装依赖
来源：http://hz.quarkkingdee.top/gtzqyglniw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.dianchejie.cn/gtkohphwuq.html

[U03] Py：加载 .env 配置
来源：http://hz.birdmap.top/gtkuirrjtd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.svipenyu.cn/gttzbrlrlg.html

[U04] Py：变量调试打印
来源：http://hz.ydzc1.top/gttaqkponp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.svipenyu.cn/gtechmepzz.html

[U05] Py：列表去重且保序
来源：http://hz.pycfn.com/gtrjkzatlg.html

list(dict.fromkeys(arr))
来源：http://hz.daria6918.cn/gtktjrinpq.html

[U06] Py：合并两个字典
来源：http://hz.tianlin.xyz/gtzgxpjxwq.html

{**a, **b}
来源：http://hz.xuetiantiany.cn/gtwbxgkpdn.html

[U07] Py：反转字典键值
来源：http://hz.yvedp.cn/gtkgwjijyy.html

{v: k for k, v in d.items()}
来源：http://hz.jlsjyb.cn/gtmkrqnzqk.html

[U08] Py：展平二维列表
来源：http://hz.yongpay.top/gtdekanksv.html

[y for x in nested for y in x]
来源：http://hz.quarkkingdee.top/gtdsbgheur.html

[U09] Py：字典取最大值的键
来源：http://hz.wangshuangyany.cn/gtusikbbpy.html

max(d, key=d.get)
来源：http://hz.fengsongda.top/gtmvgdepqi.html

[U10] Py：按值排序字典
来源：http://hz.tianlin.xyz/gtlfrmejrl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.vqdsnc.cn/gtmdkqrleo.html

[U11] Py：生成器表达式
来源：http://hz.yueranfly.top/gtozclpyxk.html

(x * 2 for x in arr)
来源：http://hz.guannengcc.top/gtxjgamtze.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhoulong.xyz/gtiudisarp.html

Counter(arr).most_common(3)
来源：http://hz.shanyushiyangtech.top/gthabmzmuf.html

[U13] Py：固定长度队列
来源：http://hz.gzhubu.top/gtawgxbizj.html

deque(maxlen=10)
来源：http://hz.gzhubu.top/gtkxnxppep.html

[U14] Py：分组收集到列表
来源：http://hz.redwolf501.top/gtlberdgoo.html

defaultdict(list)
来源：http://hz.shanyushiyangtech.top/gtbhhtozsf.html

[U15] Py：高精度计时
来源：http://hz.shangyingyoupin.top/gtoeqvatcw.html

t = time.perf_counter()
来源：http://hz.xuetiantiany.cn/gtahnzgvzt.html

[U16] Py：命令行参数解析
来源：http://hz.yongpay.top/gtzjahlbfo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.svipenyu.cn/gtfkezrlhk.html

[U17] Py：初始化日志
来源：http://hz.zhongyouzk.top/gtdukkmxjy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.vqdsnc.cn/gtwzsmphtr.html

[U18] Py：预编译正则
来源：http://hz.hongshengwenyu.top/gthmhnzkyq.html

pat = re.compile(r"\d+")
来源：http://hz.sufxvd.cn/gtmcdksach.html

[U19] Py：正则替换带回调
来源：http://hz.ppjwa.cn/gtlriwvoxr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hfpthk.cn/gteccshjbb.html

[U20] Py：缓存函数结果
来源：http://hz.52xcode.cn/gtkjkhrbsa.html

@functools.lru_cache(maxsize=None)
来源：http://hz.daria6918.cn/gtlcdeghhh.html

[U21] Py：自定义上下文管理器
来源：http://hz.gotoacloud.top/gtaqynniyz.html

@contextlib.contextmanager
来源：http://hz.jiagoushi.top/gtudikqein.html

[U22] Py：矩阵转置
来源：http://hz.gzhubu.top/gtfipadbuw.html

list(zip(*m))
来源：http://hz.jinqigufen.top/gtnytmpkco.html

[U23] Py：分块读取大文件
来源：http://hz.jianghu66.top/gtxgmpskjp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ivvv.top/gtpekkkhbw.html

[U24] Py：路径操作
来源：http://hz.hywenlv.cn/gtjdwtgxdb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hnxiangtu.top/gtpvsikslk.html

[U25] Py：CSV 按字典读
来源：http://hz.tanke756.top/gtkpevmkzv.html

csv.DictReader(f)
来源：http://hz.feifeiyinyue.top/gtrkrlzqvq.html

[U26] Py：并发下载
来源：http://hz.jyoumei.cn/gtgyptqzbx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.haohaochexian.top/gtwmrjcaom.html

[U27] Py：异步 HTTP
来源：http://hz.hfpthk.cn/gttgajrwqc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ybcxt.top/gtwcimqmrl.html

[U28] Py：类型别名
来源：http://hz.shanyushiyangkeji.top/gtblqqkbkl.html

UserId = int
来源：http://hz.zhiwuduotai.top/gtpyizwrdj.html

[U29] Py：属性校验
来源：http://hz.yj20258.top/gthrehwtvl.html

@property 与 @x.setter 配合
来源：http://hz.vqdsnc.cn/gtbznawiqy.html

[U30] Py：数据类
来源：http://hz.ywan-chungtsiang.top/gthnihezdu.html

@dataclass(slots=True)
来源：http://hz.chenlongwang.top/gtsuvpfknq.html

[U31] Py：单测
来源：http://hz.zhixingplan.top/gtfvmmzxmc.html

python -m pytest -q
来源：http://hz.jinqigufen.top/gtxijilqjh.html

[U32] Py：代码格式化
来源：http://hz.jqgufenzy.top/gtisnmrtua.html

ruff format . && ruff check --fix .
来源：http://hz.kuanghao11.cn/gtlausyihi.html

[U33] Py：打包发布
来源：http://hz.ydjk.org.cn/gtggxtfgdl.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.daria6918.cn/gtxdqtvgcy.html

[U34] Py：判断编码
来源：http://hz.jqgfzy.top/gtsfzkqvig.html

chardet.detect(raw)
来源：http://hz.kuanghao11.cn/gtqsdlzaoo.html

[U35] Py：发送邮件
来源：http://hz.aibaodan.cn/gtcipsknkk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yj20258888.top/gtmmiricvp.html

[U36] Py：定时任务
来源：http://hz.jqgfzy.top/gtxbunimeh.html

schedule.every(10).minutes.do(job)
来源：http://hz.jlsjyb.cn/gtqsevqpre.html

[U37] Py：读写 Excel
来源：http://hz.c1oappe.top/gtcorpovrt.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.dianchejie.cn/gtyhbfzmuj.html

[U38] Py：获取脚本所在目录
来源：http://hz.yj202588.top/gtktsczuno.html

Path(__file__).resolve().parent
来源：http://hz.zhiwuduotai.top/gtzobhoytn.html

[U39] Py：判断是否在交互环境
来源：http://hz.aizwys.cn/gtqfadyfqp.html

sys.stdout.isatty()
来源：http://hz.hnxiangtu.top/gtatctsimt.html

[U40] Py：打印到标准错误
来源：http://hz.ydzc1.top/gtoawbager.html

print("err", file=sys.stderr)
来源：http://hz.nanxuanxn.top/gtqpdrnyij.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.bjfxy.top/gtqwuumufz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ydjk.org.cn/gtxgxcwvfg.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.bjfxy.top/gtdtqdhnkq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gaohongyu789.top/gtdpijrsng.html

[U43] PHP：声明命名空间
来源：http://hz.hywenlv.cn/gtowjilyxk.html

namespace App\Http;
来源：http://hz.fzhhl.top/gtphtshuai.html

[U44] PHP：开启严格类型
来源：http://hz.smart0.xyz/gtyjppjgfq.html

declare(strict_types=1);
来源：http://hz.9152youxi.cn/gtfwnrzppr.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cucudq.cn/gtqsoqzkee.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yueranfly.top/gtnxctacqp.html

[U46] PHP：可空类型
来源：http://hz.yonumen.top/gtamgcrbyu.html

?string $name = null
来源：http://hz.shanyushiyangkeji.top/gtgkgsosny.html

[U47] PHP：联合类型
来源：http://hz.nwbrower.top/gtumirxdvd.html

int|string $id
来源：http://hz.hnxiangtu.top/gtqamcblie.html

[U48] PHP：纯枚举
来源：http://hz.shanyushiyangtech.top/gtuewckuih.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.meibo888.top/gtuvngfpms.html

[U49] PHP：只读属性
来源：http://hz.shuidangran.top/gtswyfodfg.html

public readonly string $name
来源：http://hz.ppjwa.cn/gthuwygbpd.html

[U50] PHP：构造器属性提升
来源：http://hz.iojbl.cn/gtiumwtrsv.html

public function __construct(private int $id) {}
来源：http://hz.andypj.xyz/gtituzoics.html

[U51] PHP：数组解构
来源：http://hz.svipenyu.cn/gtyvwvkavc.html

[$a, $b] = $arr;
来源：http://hz.ehwqpu.com/gtgxzkoxbn.html

[U52] PHP：箭头函数
来源：http://hz.yongpay.top/gtwlpysjqn.html

$double = fn($x) => $x * 2;
来源：http://hz.nwbrower.top/gturetysoj.html

[U53] PHP：空合并运算符
来源：http://hz.zhengqikj.top/gtffxeljmx.html

$v = $a ?? $b ?? "default";
来源：http://hz.shanyushiyangtech.top/gtsxzctxee.html

[U54] PHP：空安全调用
来源：http://hz.zhongyouzk.top/gtocwqdtws.html

$obj?->method()
来源：http://hz.zhongyouzk.top/gthtxdjfnb.html

[U55] PHP：match 表达式
来源：http://hz.iojbl.cn/gtyqzmerhs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.pycfn.com/gtzteukuwp.html

[U56] PHP：命名参数
来源：http://hz.havefunace.top/gtpmcozopu.html

f(a: 1, b: 2)
来源：http://hz.zhijiandao.cn/gtytxgzxpr.html

[U57] PHP：字符串插值
来源：http://hz.andypj.xyz/gtlxdirwvb.html

"值: {$a}"
来源：http://hz.xziqi.cn/gtvyteirii.html

[U58] PHP：数组三件套
来源：http://hz.cucudq.cn/gtwzcmaizx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jiagoushi.top/gtylvvruxv.html

[U59] PHP：自定义排序
来源：http://hz.fzhhl.top/gteqwgcoeg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ppjwa.cn/gtbscfccwp.html

[U60] PHP：JSON 编解码
来源：http://hz.feifeiyinyue.top/gtdgluklpp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.dianchejie.cn/gtnlufjakg.html

[U61] PHP：正则
来源：http://hz.wangshuangyany.cn/gtrfvqlnil.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtnpbzgsrf.html

[U62] PHP：日期对象
来源：http://hz.gotoacloud.top/gtamippgto.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.tianlin.xyz/gttgutnias.html

[U63] PHP：文件读写
来源：http://hz.yanxiufei.cn/gtdbilgtkt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cdnleiting.top/gtblfconwe.html

[U64] PHP：目录遍历
来源：http://hz.xuanzx.com/gtnxdihsth.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnqzz.top/gtwnyidjil.html

[U65] PHP：会话
来源：http://hz.pycfn.com/gtksitfswf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shzxlz.cn/gtydahjksq.html

[U66] PHP：设置 Cookie
来源：http://hz.cdnleiting.top/gtopolrlco.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhengqikj.top/gtkzeclrcf.html

[U67] PHP：处理文件上传
来源：http://hz.shanyushiyangkeji.top/gtkdtpnuhn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.vqdsnc.cn/gtmpxmilwr.html

[U68] PHP：PDO 连接
来源：http://hz.cucudq.cn/gtyuydrfae.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.gaohongyu789.top/gtziqdzbao.html

[U69] PHP：PDO 预处理
来源：http://hz.svipenyu.cn/gtscuzifrg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhixingplan.top/gtzmbjhanj.html

[U70] PHP：PDO 事务
来源：http://hz.ivvv.top/gtbkhsytjj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.aizwys.cn/gtcesulijs.html


<!-- 参考信息 -->