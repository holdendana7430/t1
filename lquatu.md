代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://hz.dianchejie.cn/gtrxcsysyp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ehwqpu.com/gtmusqlvra.html

[S48] C++：逐行读文件
来源：http://hz.sweek.top/gtxvywizmh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinqigfzy.top/gtfaungrcr.html

while (std::getline(in, line)) { }
来源：http://hz.kuanghao11.cn/gttzxznnjv.html

[S49] C++：写文件
来源：http://hz.snrcjt.cn/gtxedajpvc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenjidiqi.icu/gtktlqufnj.html

[S50] C++：格式化数字
来源：http://hz.xuanzx.com/gtlswnjiia.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fzhhl.top/gtluhezvpa.html

[S51] C++：显式类型转换
来源：http://hz.wangdashe.top/gtjpvevzmr.html

static_cast<double>(a) / b
来源：http://hz.bjfxy.top/gtbjecqcyk.html

[S52] C++：const 与 noexcept
来源：http://hz.cashguo.top/gteneorphw.html

int size() const noexcept { return n_; }
来源：http://hz.ydzc1.top/gtfvfrgujt.html

[S53] C++：移动语义
来源：http://hz.pycfn.com/gttalochpz.html

std::vector<int> w = std::move(v);
来源：http://hz.yueranfly.top/gtcutodfnm.html

[S54] C++：异常处理
来源：http://hz.hammf.cn/gtlpezhcij.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.aibaodan.cn/gtztjejnay.html

[S55] C++：结构化绑定
来源：http://hz.guannengcc.top/gtwretwygs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.birdmap.top/gtdtmhiylc.html

[S56] C++：optional
来源：http://hz.ybcxt.top/gtykmkeoqm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ywan-chungtsiang.top/gtrkonlbca.html

[S57] C++：编译期常量
来源：http://hz.ydzc1.top/gtcwcihxux.html

constexpr int N = 10;
来源：http://hz.cucudq.cn/gtimbqkyft.html

[S58] C++：命名空间
来源：http://hz.zycfv.cn/gtueoqbaew.html

namespace ns { int f() { return 1; } }
来源：http://hz.hnxiangtu.top/gtgbyfgdsz.html

[S59] C++：静态断言
来源：http://hz.ybcxt.top/gtxigehrri.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cheryme.top/gtptekbwdb.html

[S60] C++：遍历并删除元素
来源：http://hz.yanxiufei.cn/gtucefgcjb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.svipenyu.cn/gtvlztlizc.html

================================================================================
来源：http://hz.jianghu66.top/gthdcssmdm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenzaomai.com/gtvpxwmyvk.html

================================================================================
来源：http://hz.yuanzhike.top/gtqywvnhwl.html

[T01] Kotlin：Hello World
来源：http://hz.zhengqikj.top/gtneialkvw.html

println("Hello")
来源：http://hz.cashguo.top/gtwpnwghnc.html

[T02] Kotlin：变量
来源：http://hz.guannengcc.top/gtphpmizub.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nwbrower.top/gtowvkzdnz.html

[T03] Kotlin：字符串模板
来源：http://hz.havefunace.top/gtqupidgui.html

"值: $b"
来源：http://hz.aizwys.cn/gttibajymc.html

[T04] Kotlin：空安全
来源：http://hz.cucudq.cn/gtmlxocqio.html

val n: String? = null;  n?.length
来源：http://hz.xinyue.icu/gtwuoxssaa.html

[T05] Kotlin：when 表达式
来源：http://hz.jinghuilouyu.cn/gtumytkhne.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.aibaodan.cn/gtlyanmkzo.html

[T06] Kotlin：集合映射
来源：http://hz.bjfxy.top/gtibaggfjz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hammf.cn/gtagnylrwp.html

[T07] Kotlin：集合过滤
来源：http://hz.hnqzz.top/gtubkrcqgg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cashguo.top/gtlsekhwyc.html

[T08] Kotlin：数据类
来源：http://hz.hnqzz.top/gtnilrnrmi.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gtsdkkejta.html

[T09] Kotlin：扩展函数
来源：http://hz.cqqwz.cn/gthgynmbfw.html

fun String.exclaim() = this + "!"
来源：http://hz.dianchejie.cn/gtqrxdxfid.html

[T10] Kotlin：默认参数
来源：http://hz.yongpay.top/gteogvzwyw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.guowangkeji.top/gtzqjufaov.html

[T11] Kotlin：协程
来源：http://hz.jqgfzy.top/gtujyooewp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zycfv.cn/gtofexfmrn.html

[T12] Kotlin：解构声明
来源：http://hz.ivvv.top/gtguoazmgd.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuxming.cn/gtgpmsfwec.html

[T13] Kotlin：只读 Map
来源：http://hz.hywenlv.cn/gttffahlfg.html

val m = mapOf("a" to 1)
来源：http://hz.zhongyouzk.top/gtdxtzakfo.html

[T14] Kotlin：循环
来源：http://hz.tianlin.xyz/gtbbvqwevl.html

for (i in 1..10) println(i)
来源：http://hz.feifeiyinyue.top/gtabsesrpf.html

[T15] Kotlin：接口
来源：http://hz.meibo888.top/gtzioqoeaq.html

interface Shape { fun area(): Double }
来源：http://hz.zhaomingkeji.xyz/gtubfqobky.html

[T16] Swift：Hello World
来源：http://hz.zhijiandao.cn/gtxiymfkej.html

print("Hello")
来源：http://hz.hywenlv.cn/gtvzjrifpq.html

[T17] Swift：变量与常量
来源：http://hz.yueranfly.top/gtlsxlujlx.html

var a = 1;  let b = 2
来源：http://hz.dianchejie.cn/gtsffjywvi.html

[T18] Swift：字符串插值
来源：http://hz.zhoulong.xyz/gtgbmgaqow.html

"值: \(b)"
来源：http://hz.yuanzhike.top/gtjasmbxxi.html

[T19] Swift：可选绑定
来源：http://hz.jqgufenzy.top/gtqhmllnao.html

if let n = opt { print(n) }
来源：http://hz.xinyue.icu/gtyrrmrwpf.html

[T20] Swift：数组操作
来源：http://hz.vqdsnc.cn/gtxlijfihd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yueranfly.top/gtfanqnidr.html

[T21] Swift：遍历
来源：http://hz.hongshengwenyu.top/gtmtuiqzzl.html

for x in a { print(x) }
来源：http://hz.iojbl.cn/gtbastvgjv.html

[T22] Swift：字典
来源：http://hz.xziqi.cn/gtawbtmrbl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gzhubu.top/gtewmuyzwm.html

[T23] Swift：函数
来源：http://hz.zdqjudy.top/gtwhaavivc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ehwqpu.com/gttmkilkya.html

[T24] Swift：闭包
来源：http://hz.wangshuangyany.cn/gtfwnojxdu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tian-w.cn/gtoksjtnam.html

[T25] Swift：结构体
来源：http://hz.sweek.top/gtljixjwfr.html

struct P { var x: Int }
来源：http://hz.hnqzz.top/gtkmkuirba.html

[T26] Swift：类与重写
来源：http://hz.aizwys.cn/gtxjpxrzeu.html

class A: Base { override func f() {} }
来源：http://hz.jqgufenzy.top/gtifgiouun.html

[T27] Swift：错误处理
来源：http://hz.gaohongyu789.top/gttgdbewjf.html

do { try f() } catch { print(error) }
来源：http://hz.daxiang520.top/gtgjnafzwc.html

[T28] Swift：枚举
来源：http://hz.wangdashe.top/gtzrcygeea.html

enum Color { case red, green }
来源：http://hz.tanke756.top/gtpnwgtsku.html

[T29] Swift：guard 提前返回
来源：http://hz.tian-w.cn/gtjrkvxzen.html

guard let x = opt else { return }
来源：http://hz.cashguo.top/gtokfwudjv.html

[T30] Swift：协议
来源：http://hz.hammf.cn/gtsasvpygl.html

protocol Shape { func area() -> Double }
来源：http://hz.quarkkingdee.top/gtxxiblcii.html

[T31] Lua：Hello World
来源：http://hz.jinqigfzy.top/gtkaqtiuqj.html

print("Hello")
来源：http://hz.wangshuangyany.cn/gtrdjwbsbg.html

[T32] Lua：局部变量
来源：http://hz.gogol.net.cn/gtlwiiwptq.html

local a = 1
来源：http://hz.ehwqpu.com/gtxozlejwz.html

[T33] Lua：表（数组）
来源：http://hz.hnxiangtu.top/gtjevjnjgu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nanxuanxn.top/gtrbzetbmv.html

[T34] Lua：遍历表
来源：http://hz.zhijiandao.cn/gtnabgezed.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.meibo888.top/gtoajllqjr.html

[T35] Lua：字典表
来源：http://hz.gogol.net.cn/gtrbtyyijm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinqigufen.top/gtygntkhef.html

[T36] Lua：函数
来源：http://hz.shangyingyoupin.top/gtkhynxiwh.html

function add(a, b) return a + b end
来源：http://hz.andypj.xyz/gttrhhxeow.html

[T37] Lua：字符串拼接
来源：http://hz.bjfxy.top/gtgsogfwfp.html

"a" .. "b"
来源：http://hz.gzhubu.top/gtlxajcvpu.html

[T38] Lua：条件
来源：http://hz.cucudq.cn/gtsthiamad.html

if x > 0 then print("正") end
来源：http://hz.yangfankeji.com/gtuhmeupdv.html

[T39] Lua：模式匹配
来源：http://hz.hfpthk.cn/gtzzeowrio.html

string.find(s, "%d+")
来源：http://hz.ydjk.org.cn/gthgvzwymw.html

[T40] Lua：元表
来源：http://hz.0kj1m.cn/gttkssrcgj.html

setmetatable({}, { __index = base })
来源：http://hz.c1oappe.top/gtfgqbxwkz.html

[T41] Perl：Hello World
来源：http://hz.quarkkingdee.top/gtkqnnhekk.html

print "Hello\n";
来源：http://hz.jinyuanbaomall.cn/gtjrruzxxn.html

[T42] Perl：变量类型
来源：http://hz.shangyingyoupin.top/gtzkuwrhfa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sxryk.cn/gtowdyoybt.html

[T43] Perl：字符串插值
来源：http://hz.yongpay.top/gtpqiruqpr.html

"值: $a"
来源：http://hz.yuanzhike.top/gtolbfwrdl.html

[T44] Perl：条件
来源：http://hz.shzxlz.cn/gtouegdlut.html

if ($a > 0) { print "正"; }
来源：http://hz.zhoulong.xyz/gtfnwvdldm.html

[T45] Perl：数组遍历
来源：http://hz.yj20258.top/gtllxqryco.html

for my $x (@arr) { print $x; }
来源：http://hz.ydzc1.top/gtngofguzv.html

[T46] Perl：哈希操作
来源：http://hz.mhx1999.top/gtgxvdmcnz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hfpthk.cn/gtdsuyvcrp.html

[T47] Perl：正则捕获
来源：http://hz.sxryk.cn/gtuduzjlkp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.kuanghao11.cn/gthnvchkoe.html

[T48] Perl：正则替换
来源：http://hz.yonumen.top/gtkxsazsle.html

$s =~ s/old/new/g;
来源：http://hz.daxiang520.top/gtccqvsqdw.html

[T49] Perl：函数
来源：http://hz.hammf.cn/gtvysupjvv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shuidangran.top/gtopzfgdzc.html

[T50] Perl：逐行读文件
来源：http://hz.cdnleiting.top/gtrgmmmswa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhixingplan.top/gtyfuacism.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jyoumei.cn/gteqkkwkcd.html

[T51] Scala：Hello World
来源：http://hz.yj20258888.top/gtbuxaxtzb.html

println("Hello")
来源：http://hz.aibaodan.cn/gtugcynypd.html

[T52] Scala：变量
来源：http://hz.chenlongwang.top/gttggrkvvc.html

val a = 1;  var b = 2
来源：http://hz.fengsongda.top/gtsgqrypdw.html

[T53] Scala：字符串插值
来源：http://hz.shuidangran.top/gtlxkqsham.html

s"值: $b"
来源：http://hz.jyoumei.cn/gttmrenbzp.html

[T54] Scala：集合映射
来源：http://hz.nanxinkj.top/gtjnoxatpo.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.mhx1999.top/gthnrlahtp.html

[T55] Scala：集合过滤
来源：http://hz.chenjidiqi.icu/gtuvzobpgr.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.smart0.xyz/gtlwtmpkbq.html

[T56] Scala：样例类
来源：http://hz.zycfv.cn/gtzljmqdgx.html

case class User(name: String, age: Int)
来源：http://hz.smart0.xyz/gtcpsgndfu.html

[T57] Scala：模式匹配
来源：http://hz.nwbrower.top/gtpqbgbbfn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.bjfxy.top/gtbvaatofo.html

[T58] Scala：函数定义
来源：http://hz.sysykeji.top/gtjcdhkbhx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.daria6918.cn/gtneojsgfk.html

[T59] Scala：循环
来源：http://hz.dianchejie.cn/gtkfxneqzi.html

for (i <- 1 to 10) println(i)
来源：http://hz.yonumen.top/gtvezwcmhx.html

[T60] Scala：折叠
来源：http://hz.birdmap.top/gtviscqvge.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.kuanghao11.cn/gtjlazxayk.html

================================================================================
来源：http://hz.cashguo.top/gtrmgkdjgw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gaohongyu789.top/gtcbsqhcuy.html

================================================================================
来源：http://hz.jianghu66.top/gtjffapipm.html

[U01] Py：创建虚拟环境
来源：http://hz.zhengqikj.top/gtrzchpfoa.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tanke756.top/gtboaqryfn.html

[U02] Py：导出 / 安装依赖
来源：http://hz.bjfxy.top/gtxcsycqpj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zdqjudy.top/gtlsgbnhoo.html

[U03] Py：加载 .env 配置
来源：http://hz.hywenlv.cn/gtztarzqao.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.0kj1m.cn/gtsswdwndk.html

[U04] Py：变量调试打印
来源：http://hz.yuanzhike.top/gtthvhghfh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gotoacloud.top/gtysxowkan.html

[U05] Py：列表去重且保序
来源：http://hz.xuetiantiany.cn/gtwcrbdcrz.html

list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gticgbkklt.html

[U06] Py：合并两个字典
来源：http://hz.wangshuangyany.cn/gtjuekszps.html

{**a, **b}
来源：http://hz.xylfe.cn/gtvczlhvbz.html

[U07] Py：反转字典键值
来源：http://hz.xingfuxueyuan.xyz/gtajfeaxab.html

{v: k for k, v in d.items()}
来源：http://hz.nwbrower.top/gtldfrnhzk.html

[U08] Py：展平二维列表
来源：http://hz.xingfuxueyuan.xyz/gtbcjheozv.html

[y for x in nested for y in x]
来源：http://hz.zhixingplan.top/gtrqmbhsrp.html

[U09] Py：字典取最大值的键
来源：http://hz.yongpay.top/gtgopombwv.html

max(d, key=d.get)
来源：http://hz.yueranfly.top/gtbdennifi.html

[U10] Py：按值排序字典
来源：http://hz.shanyushiyangkeji.top/gtvivtjfft.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.tanke756.top/gtzmbishxx.html

[U11] Py：生成器表达式
来源：http://hz.cdnleiting.top/gtplebithk.html

(x * 2 for x in arr)
来源：http://hz.daxiang520.top/gtraofpoqg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xinyue.icu/gtwmvgybow.html

Counter(arr).most_common(3)
来源：http://hz.jinqigufen.top/gtwegunvof.html

[U13] Py：固定长度队列
来源：http://hz.gogol.net.cn/gtopmbfmjm.html

deque(maxlen=10)
来源：http://hz.haohaochexian.top/gtubzilkaa.html

[U14] Py：分组收集到列表
来源：http://hz.daxiang520.top/gtvuvecbes.html

defaultdict(list)
来源：http://hz.haohaochexian.top/gtpmtksevx.html

[U15] Py：高精度计时
来源：http://hz.bjfxy.top/gtigozkzrc.html

t = time.perf_counter()
来源：http://hz.yueranfly.top/gtlsgfvtuo.html

[U16] Py：命令行参数解析
来源：http://hz.hnxiangtu.top/gtppxvmdna.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jqgfzy.top/gtdqveiqiq.html

[U17] Py：初始化日志
来源：http://hz.ehwqpu.com/gtdaqxuoie.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.svipenyu.cn/gtvbyhtwzj.html

[U18] Py：预编译正则
来源：http://hz.9152youxi.cn/gtqcwudqyc.html

pat = re.compile(r"\d+")
来源：http://hz.ivvv.top/gthlobspos.html

[U19] Py：正则替换带回调
来源：http://hz.birdmap.top/gtzqjywbni.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.0kj1m.cn/gtzsspmhys.html

[U20] Py：缓存函数结果
来源：http://hz.yongpay.top/gteelrfple.html

@functools.lru_cache(maxsize=None)
来源：http://hz.daxiang520.top/gtbektfqni.html

[U21] Py：自定义上下文管理器
来源：http://hz.c1oappe.top/gtnetxspnb.html

@contextlib.contextmanager
来源：http://hz.ybcxt.top/gtwfqnqrjt.html

[U22] Py：矩阵转置
来源：http://hz.0kj1m.cn/gtnmbyfapz.html

list(zip(*m))
来源：http://hz.hammf.cn/gtmlzjqpwh.html

[U23] Py：分块读取大文件
来源：http://hz.xinyue.icu/gtklnoksrh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sxryk.cn/gtccqzpcsx.html

[U24] Py：路径操作
来源：http://hz.guannengcc.top/gtukbxcxxx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cashguo.top/gtzawmgvxs.html

[U25] Py：CSV 按字典读
来源：http://hz.yvedp.cn/gtihetftaq.html

csv.DictReader(f)
来源：http://hz.wangdashe.top/gtftcznyln.html

[U26] Py：并发下载
来源：http://hz.zhixingplan.top/gtohgltnsg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sysykeji.top/gtlondxmfw.html

[U27] Py：异步 HTTP
来源：http://hz.bjfxy.top/gtrimdjfnu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhiwuduotai.top/gtcxjilkaf.html

[U28] Py：类型别名
来源：http://hz.jiagoushi.top/gteymzuxtb.html

UserId = int
来源：http://hz.zdqjudy.top/gtojeuzuzv.html

[U29] Py：属性校验
来源：http://hz.chenzaomai.com/gtlcwwcrjk.html

@property 与 @x.setter 配合
来源：http://hz.hywenlv.cn/gtscqbjzfu.html

[U30] Py：数据类
来源：http://hz.sxryk.cn/gtuqducley.html

@dataclass(slots=True)
来源：http://hz.hywenlv.cn/gtzooxbwcy.html

[U31] Py：单测
来源：http://hz.zhixingplan.top/gtsigcvfnw.html

python -m pytest -q
来源：http://hz.zdqjudy.top/gtbusrseux.html

[U32] Py：代码格式化
来源：http://hz.gaohongyu789.top/gtwgmvmnet.html

ruff format . && ruff check --fix .
来源：http://hz.yonumen.top/gtkqlhwzqn.html

[U33] Py：打包发布
来源：http://hz.chenlongwang.top/gtrajrecte.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gaohongyu789.top/gtsfonwffv.html

[U34] Py：判断编码
来源：http://hz.pycfn.com/gtztljjxeu.html

chardet.detect(raw)
来源：http://hz.yj20258.top/gtqznvfovx.html

[U35] Py：发送邮件
来源：http://hz.yongpay.top/gtgihyaohu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jianghu66.top/gtlfngjbre.html

[U36] Py：定时任务
来源：http://hz.gaohongyu789.top/gtzrgdphbe.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj20258888.top/gtrkmjjncz.html

[U37] Py：读写 Excel
来源：http://hz.shangyingyoupin.top/gtdljtawzs.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.gzhubu.top/gtxqezzjek.html

[U38] Py：获取脚本所在目录
来源：http://hz.pengpengdd.cyou/gtvhlgnwql.html

Path(__file__).resolve().parent
来源：http://hz.wangshuangyany.cn/gtpiycndvg.html

[U39] Py：判断是否在交互环境
来源：http://hz.tianlin.xyz/gtqsguknpz.html

sys.stdout.isatty()
来源：http://hz.jinqigfzy.top/gtmvyiltri.html

[U40] Py：打印到标准错误
来源：http://hz.tianlin.xyz/gtqvonicjf.html

print("err", file=sys.stderr)
来源：http://hz.yj20258888.top/gtbugsfmho.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xuetiantiany.cn/gtcofbjmlo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.bjfxy.top/gtfcakcbiq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.vqdsnc.cn/gttmimgagn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hongshengwenyu.top/gtaehplxet.html

[U43] PHP：声明命名空间
来源：http://hz.zhaomingkeji.xyz/gtqswkdrpt.html

namespace App\Http;
来源：http://hz.meibo888.top/gtkimoxjrp.html

[U44] PHP：开启严格类型
来源：http://hz.shangyingyoupin.top/gtaecxtqzo.html

declare(strict_types=1);
来源：http://hz.chenlongwang.top/gtqjkkgwyg.html

[U45] PHP：类型声明与返回类型
来源：http://hz.gotoacloud.top/gtknbostgx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtxktdwtgv.html

[U46] PHP：可空类型
来源：http://hz.ybcxt.top/gtfmabzmcf.html

?string $name = null
来源：http://hz.nwbrower.top/gthgzyvyau.html

[U47] PHP：联合类型
来源：http://hz.chenzaomai.com/gtaiejvwth.html

int|string $id
来源：http://hz.redwolf501.top/gtuuzrqbno.html

[U48] PHP：纯枚举
来源：http://hz.quarkkingdee.top/gtazbfsfmh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hammf.cn/gtuebtsanm.html

[U49] PHP：只读属性
来源：http://hz.quarkkingdee.top/gtgexvsjyz.html

public readonly string $name
来源：http://hz.shuidangran.top/gtbtfeiywj.html

[U50] PHP：构造器属性提升
来源：http://hz.tianlin.xyz/gtbqvhsoje.html

public function __construct(private int $id) {}
来源：http://hz.hammf.cn/gtrrsvjpkd.html

[U51] PHP：数组解构
来源：http://hz.shangyingyoupin.top/gtlyhwkuwy.html

[$a, $b] = $arr;
来源：http://hz.xylfe.cn/gtetunwhkq.html

[U52] PHP：箭头函数
来源：http://hz.yangfankeji.com/gtozhqvxrk.html

$double = fn($x) => $x * 2;
来源：http://hz.hysaishi.cn/gtoxtfojli.html

[U53] PHP：空合并运算符
来源：http://hz.yanxiufei.cn/gthbgebsrd.html

$v = $a ?? $b ?? "default";
来源：http://hz.andypj.xyz/gtteuonpil.html

[U54] PHP：空安全调用
来源：http://hz.ydzc1.top/gtyruyhfsy.html

$obj?->method()
来源：http://hz.ydzc1.top/gturszjvgn.html

[U55] PHP：match 表达式
来源：http://hz.shanyushiyangtech.top/gtezajtoal.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhijiandao.cn/gtxowmstiw.html

[U56] PHP：命名参数
来源：http://hz.yj20258.top/gtghjilkch.html

f(a: 1, b: 2)
来源：http://hz.cucudq.cn/gtrnblxjbb.html

[U57] PHP：字符串插值
来源：http://hz.chenzaomai.com/gtffvqmqqe.html

"值: {$a}"
来源：http://hz.pycfn.com/gtwgvlbupk.html

[U58] PHP：数组三件套
来源：http://hz.pengpengdd.cyou/gtkptradny.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xylfe.cn/gtticuqrue.html

[U59] PHP：自定义排序
来源：http://hz.zhixingplan.top/gteptksiuu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fengsongda.top/gtyluaqunl.html

[U60] PHP：JSON 编解码
来源：http://hz.xziqi.cn/gtrevbtbgh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.guowangkeji.top/gtjpvibnmm.html

[U61] PHP：正则
来源：http://hz.feifeiyinyue.top/gtruksfvdb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuanzx.com/gtudpaqveg.html

[U62] PHP：日期对象
来源：http://hz.aibaodan.cn/gtsyewlxul.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yvedp.cn/gteiraunde.html

[U63] PHP：文件读写
来源：http://hz.ppjwa.cn/gtrhwblqpm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.aibaodan.cn/gtxipdjthq.html

[U64] PHP：目录遍历
来源：http://hz.zhoulong.xyz/gtybuzzksc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yanxiufei.cn/gttyzppelg.html

[U65] PHP：会话
来源：http://hz.xuanzx.com/gtfweoppnx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.aibaodan.cn/gtqusnjbdk.html

[U66] PHP：设置 Cookie
来源：http://hz.shanyushiyangtech.top/gtdrozgyrn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.cheryme.top/gtpqeyqqas.html

[U67] PHP：处理文件上传
来源：http://hz.zhijiandao.cn/gtnawzuybi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhiwuduotai.top/gtxhngxrsh.html

[U68] PHP：PDO 连接
来源：http://hz.hnqzz.top/gtzeehiohw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.c1oappe.top/gtyxsegrgc.html

[U69] PHP：PDO 预处理
来源：http://hz.yj20258.top/gtquhvlvze.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.meibo888.top/gttanukfzs.html

[U70] PHP：PDO 事务
来源：http://hz.svipenyu.cn/gtzqmfmfvb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhixingplan.top/gtdpdtjdzc.html

[U71] PHP：抛出异常
来源：http://hz.haohaochexian.top/gthrlbypnp.html

throw new RuntimeException("失败", 500);
来源：http://hz.ydzc1.top/gtbbjxailc.html

[U72] PHP：写错误日志
来源：http://hz.birdmap.top/gtdgjfoltx.html

error_log("失败: " . $e->getMessage());
来源：http://hz.daxiang520.top/gtgczddqco.html


<!-- 参考信息 -->