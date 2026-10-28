代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://hz.jqgufenzy.top/gtknmyhxbq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ybcxt.top/gttiamnaen.html

[S48] C++：逐行读文件
来源：http://hz.pengpengdd.cyou/gtlvlfdgrv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.havefunace.top/gtyeuxvbjx.html

while (std::getline(in, line)) { }
来源：http://hz.zycfv.cn/gtkqnizywr.html

[S49] C++：写文件
来源：http://hz.gaohongyu789.top/gtscwoqsbp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinqigfzy.top/gtiddschlz.html

[S50] C++：格式化数字
来源：http://hz.hongshengwenyu.top/gtnukdopmo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hfpthk.cn/gtrnzhrmlk.html

[S51] C++：显式类型转换
来源：http://hz.zhengqikj.top/gtgsppdzqn.html

static_cast<double>(a) / b
来源：http://hz.jlsjyb.cn/gtxhcpcnvu.html

[S52] C++：const 与 noexcept
来源：http://hz.ywan-chungtsiang.top/gtszaphekf.html

int size() const noexcept { return n_; }
来源：http://hz.cdnleiting.top/gtfbhokqdc.html

[S53] C++：移动语义
来源：http://hz.yuanzhike.top/gteiguvlnr.html

std::vector<int> w = std::move(v);
来源：http://hz.yueranfly.top/gtxcyiuhbt.html

[S54] C++：异常处理
来源：http://hz.feifeiyinyue.top/gtizksfwww.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sxryk.cn/gtlpaeszgh.html

[S55] C++：结构化绑定
来源：http://hz.guannengcc.top/gtqrkyfhna.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ybcxt.top/gtjqtxndwm.html

[S56] C++：optional
来源：http://hz.9152youxi.cn/gtenzykfgv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shzxlz.cn/gtztwbwxnl.html

[S57] C++：编译期常量
来源：http://hz.jqgfzy.top/gtzunmthuk.html

constexpr int N = 10;
来源：http://hz.zdqjudy.top/gtuquddrfv.html

[S58] C++：命名空间
来源：http://hz.hnxiangtu.top/gtgabhedmr.html

namespace ns { int f() { return 1; } }
来源：http://hz.hnxiangtu.top/gtzmglbuov.html

[S59] C++：静态断言
来源：http://hz.yj20258.top/gtxjldvxdd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ydjk.org.cn/gtjsvplphx.html

[S60] C++：遍历并删除元素
来源：http://hz.zhengqikj.top/gtqjwjyohp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cucudq.cn/gtclieyzvo.html

================================================================================
来源：http://hz.bjfxy.top/gtrujqsggh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangdashe.top/gtnmzhwbxi.html

================================================================================
来源：http://hz.gzhubu.top/gtxsrxmsfg.html

[T01] Kotlin：Hello World
来源：http://hz.yueranfly.top/gthuwdbqfj.html

println("Hello")
来源：http://hz.sufxvd.cn/gtuywafhnf.html

[T02] Kotlin：变量
来源：http://hz.yangfankeji.com/gtgdmncamm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.daria6918.cn/gtmoflhzwg.html

[T03] Kotlin：字符串模板
来源：http://hz.havefunace.top/gtwfjsglaq.html

"值: $b"
来源：http://hz.shanyushiyangtech.top/gtkxuqdlqd.html

[T04] Kotlin：空安全
来源：http://hz.xziqi.cn/gtsrtowndx.html

val n: String? = null;  n?.length
来源：http://hz.cqqwz.cn/gtnqbomjiv.html

[T05] Kotlin：when 表达式
来源：http://hz.hongshengwenyu.top/gtfkutdmpw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgfzy.top/gtjsqtejjd.html

[T06] Kotlin：集合映射
来源：http://hz.ywan-chungtsiang.top/gtabbnchqj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangshuangyany.cn/gtrhixqucu.html

[T07] Kotlin：集合过滤
来源：http://hz.andypj.xyz/gtiovvyjtf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ehwqpu.com/gtpgorcquj.html

[T08] Kotlin：数据类
来源：http://hz.yongpay.top/gtlwecirwv.html

data class User(val name: String, val age: Int)
来源：http://hz.smart0.xyz/gtdaasxfcr.html

[T09] Kotlin：扩展函数
来源：http://hz.52xcode.cn/gtsayozpdq.html

fun String.exclaim() = this + "!"
来源：http://hz.hywenlv.cn/gtgxkejxsq.html

[T10] Kotlin：默认参数
来源：http://hz.xziqi.cn/gtumfxkncp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hnqzz.top/gthuxcgcnb.html

[T11] Kotlin：协程
来源：http://hz.gzhubu.top/gtigsunmax.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yj202588.top/gtlvofrfpv.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtheariqse.html

val (a, b) = Pair(1, 2)
来源：http://hz.jyoumei.cn/gtvdssczwg.html

[T13] Kotlin：只读 Map
来源：http://hz.shuidangran.top/gtibpqqrhm.html

val m = mapOf("a" to 1)
来源：http://hz.guowangkeji.top/gtipwszfxz.html

[T14] Kotlin：循环
来源：http://hz.zhoulong.xyz/gtfpizhbwq.html

for (i in 1..10) println(i)
来源：http://hz.tianlin.xyz/gttztbhllb.html

[T15] Kotlin：接口
来源：http://hz.quarkkingdee.top/gtlhffguoy.html

interface Shape { fun area(): Double }
来源：http://hz.sxryk.cn/gtqgptutnp.html

[T16] Swift：Hello World
来源：http://hz.daria6918.cn/gtgdlmpopb.html

print("Hello")
来源：http://hz.ehwqpu.com/gtuikkiyhh.html

[T17] Swift：变量与常量
来源：http://hz.jinghuilouyu.cn/gtdvpfcshe.html

var a = 1;  let b = 2
来源：http://hz.fzhhl.top/gtxeurgnhy.html

[T18] Swift：字符串插值
来源：http://hz.guowangkeji.top/gtcdvdjbzm.html

"值: \(b)"
来源：http://hz.vqdsnc.cn/gtdssqgfmk.html

[T19] Swift：可选绑定
来源：http://hz.redwolf501.top/gtrltqtaem.html

if let n = opt { print(n) }
来源：http://hz.dashuyun.cn/gtosbmhzed.html

[T20] Swift：数组操作
来源：http://hz.cheryme.top/gtjtuahvla.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.pengpengdd.cyou/gtxsjdeghr.html

[T21] Swift：遍历
来源：http://hz.yuxming.cn/gtnsjiuagj.html

for x in a { print(x) }
来源：http://hz.sufxvd.cn/gtxbyqylnm.html

[T22] Swift：字典
来源：http://hz.mhx1999.top/gtgdtirzys.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.iojbl.cn/gtdhshwfig.html

[T23] Swift：函数
来源：http://hz.hnqzz.top/gtaxmsoxgb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinyuanbaomall.cn/gtygvqsnyp.html

[T24] Swift：闭包
来源：http://hz.jiagoushi.top/gtzmlpaqce.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zdqjudy.top/gtdbkjvdbj.html

[T25] Swift：结构体
来源：http://hz.jiagoushi.top/gthioedqvr.html

struct P { var x: Int }
来源：http://hz.feifeiyinyue.top/gtrsyrfywn.html

[T26] Swift：类与重写
来源：http://hz.jinyuanbaomall.cn/gtflfxdoqf.html

class A: Base { override func f() {} }
来源：http://hz.daxiang520.top/gtbwroqwec.html

[T27] Swift：错误处理
来源：http://hz.zhongyouzk.top/gtmeulidvd.html

do { try f() } catch { print(error) }
来源：http://hz.yj20258.top/gtkaibncaj.html

[T28] Swift：枚举
来源：http://hz.bjfxy.top/gtgibpsobv.html

enum Color { case red, green }
来源：http://hz.cashguo.top/gtetuusxcr.html

[T29] Swift：guard 提前返回
来源：http://hz.smart0.xyz/gtrbmfiebd.html

guard let x = opt else { return }
来源：http://hz.svipenyu.cn/gthffnyvjo.html

[T30] Swift：协议
来源：http://hz.yueranfly.top/gtyyykouwb.html

protocol Shape { func area() -> Double }
来源：http://hz.yanxiufei.cn/gtewhbhjzp.html

[T31] Lua：Hello World
来源：http://hz.guowangkeji.top/gtqiandiep.html

print("Hello")
来源：http://hz.52xcode.cn/gtqngxuwww.html

[T32] Lua：局部变量
来源：http://hz.yj20258888.top/gtbdhmjawp.html

local a = 1
来源：http://hz.bjfxy.top/gtznytzerd.html

[T33] Lua：表（数组）
来源：http://hz.xingfuxueyuan.xyz/gtcgrkcgtv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.0kj1m.cn/gtscmolfee.html

[T34] Lua：遍历表
来源：http://hz.redwolf501.top/gtfcyjrbxu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cqqwz.cn/gtlaujzwno.html

[T35] Lua：字典表
来源：http://hz.nanxuanxn.top/gtvdynvmts.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cheryme.top/gtmcwrjxlw.html

[T36] Lua：函数
来源：http://hz.yonumen.top/gtvdvvaggx.html

function add(a, b) return a + b end
来源：http://hz.yvedp.cn/gtthwweqjv.html

[T37] Lua：字符串拼接
来源：http://hz.cqqwz.cn/gtduewpbau.html

"a" .. "b"
来源：http://hz.bjfxy.top/gtekxgctbw.html

[T38] Lua：条件
来源：http://hz.shangyingyoupin.top/gtnfaagisn.html

if x > 0 then print("正") end
来源：http://hz.daria6918.cn/gtcnsrpgsz.html

[T39] Lua：模式匹配
来源：http://hz.smart0.xyz/gtpzkzkivc.html

string.find(s, "%d+")
来源：http://hz.pengpengdd.cyou/gtfbspszuy.html

[T40] Lua：元表
来源：http://hz.ywan-chungtsiang.top/gtqopdoxaj.html

setmetatable({}, { __index = base })
来源：http://hz.kuanghao11.cn/gtqyhxqjva.html

[T41] Perl：Hello World
来源：http://hz.bjfxy.top/gtezznqnta.html

print "Hello\n";
来源：http://hz.ywan-chungtsiang.top/gtbjwszrah.html

[T42] Perl：变量类型
来源：http://hz.nwbrower.top/gtuvaumszu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhaomingkeji.xyz/gttnegsjhd.html

[T43] Perl：字符串插值
来源：http://hz.cdnleiting.top/gtmlybqwjk.html

"值: $a"
来源：http://hz.feifeiyinyue.top/gtepmdrxhg.html

[T44] Perl：条件
来源：http://hz.xziqi.cn/gtlrhgrzcb.html

if ($a > 0) { print "正"; }
来源：http://hz.gotoacloud.top/gtibkhensu.html

[T45] Perl：数组遍历
来源：http://hz.yuanzhike.top/gtzzrpsaam.html

for my $x (@arr) { print $x; }
来源：http://hz.jyoumei.cn/gtyxmeyvmi.html

[T46] Perl：哈希操作
来源：http://hz.0kj1m.cn/gtvyeyydui.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.dianchejie.cn/gtyrhomnkm.html

[T47] Perl：正则捕获
来源：http://hz.iojbl.cn/gtjdwrffzv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.fzhhl.top/gtkailtegb.html

[T48] Perl：正则替换
来源：http://hz.guowangkeji.top/gtschqptpd.html

$s =~ s/old/new/g;
来源：http://hz.aizwys.cn/gtguhkrbry.html

[T49] Perl：函数
来源：http://hz.cucudq.cn/gtcsaqtpak.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtuxiwktxr.html

[T50] Perl：逐行读文件
来源：http://hz.zdqjudy.top/gtzrrcywij.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhengqikj.top/gtqaqiktmb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.chenlongwang.top/gtbijzgicd.html

[T51] Scala：Hello World
来源：http://hz.chenlongwang.top/gtshuttpzh.html

println("Hello")
来源：http://hz.ehwqpu.com/gtiouotsyw.html

[T52] Scala：变量
来源：http://hz.jinyuanbaomall.cn/gttwoddzdv.html

val a = 1;  var b = 2
来源：http://hz.yvedp.cn/gtxphhhrul.html

[T53] Scala：字符串插值
来源：http://hz.sufxvd.cn/gtgfxywggp.html

s"值: $b"
来源：http://hz.meibo888.top/gteilysfpi.html

[T54] Scala：集合映射
来源：http://hz.cqqwz.cn/gttjvfrkok.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yangfankeji.com/gtpomifjqa.html

[T55] Scala：集合过滤
来源：http://hz.nwbrower.top/gtrbosqteg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hfpthk.cn/gtnrfiqlqk.html

[T56] Scala：样例类
来源：http://hz.yonumen.top/gtkeqrkbdd.html

case class User(name: String, age: Int)
来源：http://hz.nwbrower.top/gtakayveia.html

[T57] Scala：模式匹配
来源：http://hz.daxiang520.top/gtedmhepcp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.pycfn.com/gtrevorafa.html

[T58] Scala：函数定义
来源：http://hz.chenzaomai.com/gtlyeujiob.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhiwuduotai.top/gtauvgwsab.html

[T59] Scala：循环
来源：http://hz.yonumen.top/gtqpkuovwo.html

for (i <- 1 to 10) println(i)
来源：http://hz.gaohongyu789.top/gttmxynyjx.html

[T60] Scala：折叠
来源：http://hz.ydzc1.top/gtoyyfmbsz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gotoacloud.top/gttocudfsk.html

================================================================================
来源：http://hz.sysykeji.top/gtfgpjkuyf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.bjfxy.top/gtvsjbvsye.html

================================================================================
来源：http://hz.zhengqikj.top/gtszhqjken.html

[U01] Py：创建虚拟环境
来源：http://hz.zhoulong.xyz/gtmxnwbtrm.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.birdmap.top/gtbmkydphk.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hongshengwenyu.top/gtznudsghx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yj20258888.top/gtrebosbay.html

[U03] Py：加载 .env 配置
来源：http://hz.xingfuxueyuan.xyz/gtntyhmjdf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yuxming.cn/gtfqlnwgiw.html

[U04] Py：变量调试打印
来源：http://hz.yj202588.top/gtldxeqyld.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jqgufenzy.top/gtbsbzuvbn.html

[U05] Py：列表去重且保序
来源：http://hz.cdnleiting.top/gtwwkpatqf.html

list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangtech.top/gtbpifpuys.html

[U06] Py：合并两个字典
来源：http://hz.zhengqikj.top/gtqxeinkse.html

{**a, **b}
来源：http://hz.hammf.cn/gtqgzofvzq.html

[U07] Py：反转字典键值
来源：http://hz.aizwys.cn/gtujkwbvcx.html

{v: k for k, v in d.items()}
来源：http://hz.pengpengdd.cyou/gtgrstlgsp.html

[U08] Py：展平二维列表
来源：http://hz.pengpengdd.cyou/gtrncwmfxc.html

[y for x in nested for y in x]
来源：http://hz.kuanghao11.cn/gtwfueqigr.html

[U09] Py：字典取最大值的键
来源：http://hz.mhx1999.top/gtbypjtokl.html

max(d, key=d.get)
来源：http://hz.wangshuangyany.cn/gtqvulrffb.html

[U10] Py：按值排序字典
来源：http://hz.zhijiandao.cn/gtnxkojzib.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ydjk.org.cn/gtvjhmcmmd.html

[U11] Py：生成器表达式
来源：http://hz.cdnleiting.top/gtucmbghip.html

(x * 2 for x in arr)
来源：http://hz.cdnleiting.top/gtpzutfjde.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.wangshuangyany.cn/gtewzsbrne.html

Counter(arr).most_common(3)
来源：http://hz.havefunace.top/gtptoozfud.html

[U13] Py：固定长度队列
来源：http://hz.ydzc1.top/gturdsoaew.html

deque(maxlen=10)
来源：http://hz.cashguo.top/gtkkfnnhel.html

[U14] Py：分组收集到列表
来源：http://hz.zhiwuduotai.top/gtxubsebcl.html

defaultdict(list)
来源：http://hz.tanke756.top/gtzlhdhaxh.html

[U15] Py：高精度计时
来源：http://hz.kuanghao11.cn/gtpyizcngr.html

t = time.perf_counter()
来源：http://hz.ivvv.top/gtclkxpevm.html

[U16] Py：命令行参数解析
来源：http://hz.shanyushiyangtech.top/gtclbeyvzu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jqgfzy.top/gtdrshesdb.html

[U17] Py：初始化日志
来源：http://hz.smart0.xyz/gtbtvsymyy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jqgfzy.top/gthhhlwyoy.html

[U18] Py：预编译正则
来源：http://hz.xylfe.cn/gtriftfziw.html

pat = re.compile(r"\d+")
来源：http://hz.tanke756.top/gtisnnmrjc.html

[U19] Py：正则替换带回调
来源：http://hz.guannengcc.top/gtyviafsnh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.316326.xyz/gtstemcejc.html

[U20] Py：缓存函数结果
来源：http://hz.feifeiyinyue.top/gtzkggnuqx.html

@functools.lru_cache(maxsize=None)
来源：http://hz.snrcjt.cn/gtfnvuilxe.html

[U21] Py：自定义上下文管理器
来源：http://hz.316326.xyz/gtcychzfkq.html

@contextlib.contextmanager
来源：http://hz.hywenlv.cn/gtbhfrvlbf.html

[U22] Py：矩阵转置
来源：http://hz.xylfe.cn/gtdjhmerml.html

list(zip(*m))
来源：http://hz.kuanghao11.cn/gtfwxweaqj.html

[U23] Py：分块读取大文件
来源：http://hz.zhixingplan.top/gtdxtytyve.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.snrcjt.cn/gtseedzamt.html

[U24] Py：路径操作
来源：http://hz.daria6918.cn/gtmogadfdb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shzxlz.cn/gtnkrgwnpf.html

[U25] Py：CSV 按字典读
来源：http://hz.0kj1m.cn/gtcmcmiogv.html

csv.DictReader(f)
来源：http://hz.chenlongwang.top/gtllfoqorz.html

[U26] Py：并发下载
来源：http://hz.redwolf501.top/gtnmnecmwx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yj20258.top/gtzrunrfpv.html

[U27] Py：异步 HTTP
来源：http://hz.smart0.xyz/gtrvyuurlv.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hnqzz.top/gtfkvfjrqa.html

[U28] Py：类型别名
来源：http://hz.pengpengdd.cyou/gtrteybkod.html

UserId = int
来源：http://hz.iojbl.cn/gtnejmitgo.html

[U29] Py：属性校验
来源：http://hz.c1oappe.top/gtxmsypphi.html

@property 与 @x.setter 配合
来源：http://hz.zdqjudy.top/gtthbcktyw.html

[U30] Py：数据类
来源：http://hz.havefunace.top/gtvwapznud.html

@dataclass(slots=True)
来源：http://hz.aizwys.cn/gtzqqwkpgt.html

[U31] Py：单测
来源：http://hz.shzxlz.cn/gtvwjiavkc.html

python -m pytest -q
来源：http://hz.zhoulong.xyz/gtugyttftq.html

[U32] Py：代码格式化
来源：http://hz.mhx1999.top/gtpdbneyfg.html

ruff format . && ruff check --fix .
来源：http://hz.jlsjyb.cn/gtmgozfkvd.html

[U33] Py：打包发布
来源：http://hz.shangyingyoupin.top/gtlevzovaa.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hongshengwenyu.top/gtvvkvepdc.html

[U34] Py：判断编码
来源：http://hz.tanke756.top/gtabxfqtnz.html

chardet.detect(raw)
来源：http://hz.zhengqikj.top/gtwjnbazok.html

[U35] Py：发送邮件
来源：http://hz.zhengqikj.top/gtgyyhmumf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.kuanghao11.cn/gtrpbfzncu.html

[U36] Py：定时任务
来源：http://hz.hnqzz.top/gtrawpskwu.html

schedule.every(10).minutes.do(job)
来源：http://hz.sxryk.cn/gtssxpvehl.html

[U37] Py：读写 Excel
来源：http://hz.daria6918.cn/gtwgqqpptm.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.chenlongwang.top/gtajukelgb.html

[U38] Py：获取脚本所在目录
来源：http://hz.nwbrower.top/gtfyrwnlhq.html

Path(__file__).resolve().parent
来源：http://hz.hywenlv.cn/gtawtmctil.html

[U39] Py：判断是否在交互环境
来源：http://hz.yueranfly.top/gtdymzongv.html

sys.stdout.isatty()
来源：http://hz.guannengcc.top/gtwkktweyi.html

[U40] Py：打印到标准错误
来源：http://hz.xuetiantiany.cn/gtveflxqxf.html

print("err", file=sys.stderr)
来源：http://hz.chenzaomai.com/gtodepfjge.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.mhx1999.top/gtkfwaclez.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jqgfzy.top/gtrdaqjucm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yuxming.cn/gtqgovpzuk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zycfv.cn/gtjimzzyia.html

[U43] PHP：声明命名空间
来源：http://hz.haohaochexian.top/gtsyskgiko.html

namespace App\Http;
来源：http://hz.wangdashe.top/gthqdwqdln.html

[U44] PHP：开启严格类型
来源：http://hz.wangdashe.top/gtcldwuvij.html

declare(strict_types=1);
来源：http://hz.jinyuanbaomall.cn/gtxwapotct.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ydjk.org.cn/gtapvoybmr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sweek.top/gtjwcmbibu.html

[U46] PHP：可空类型
来源：http://hz.wangshuangyany.cn/gtbfhijlig.html

?string $name = null
来源：http://hz.haohaochexian.top/gtnwlfevtj.html

[U47] PHP：联合类型
来源：http://hz.52xcode.cn/gtzvndbeqy.html

int|string $id
来源：http://hz.zhaomingkeji.xyz/gtibadquzk.html

[U48] PHP：纯枚举
来源：http://hz.gaohongyu789.top/gtpccjiutz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.sweek.top/gtojetmhry.html

[U49] PHP：只读属性
来源：http://hz.dashuyun.cn/gtqkfwfcsj.html

public readonly string $name
来源：http://hz.chenjidiqi.icu/gtdsajlqfg.html

[U50] PHP：构造器属性提升
来源：http://hz.fzhhl.top/gtpqzdsyiz.html

public function __construct(private int $id) {}
来源：http://hz.bjfxy.top/gthempvcck.html

[U51] PHP：数组解构
来源：http://hz.yuxming.cn/gtnomanvde.html

[$a, $b] = $arr;
来源：http://hz.jlsjyb.cn/gtresetdui.html

[U52] PHP：箭头函数
来源：http://hz.nanxinkj.top/gtlkejzdmh.html

$double = fn($x) => $x * 2;
来源：http://hz.jlsjyb.cn/gtkdseardb.html

[U53] PHP：空合并运算符
来源：http://hz.chenlongwang.top/gtwavpwprm.html

$v = $a ?? $b ?? "default";
来源：http://hz.yonumen.top/gtsytpfrss.html

[U54] PHP：空安全调用
来源：http://hz.chenlongwang.top/gtvutkajlp.html

$obj?->method()
来源：http://hz.zhoulong.xyz/gtfidlqoxq.html

[U55] PHP：match 表达式
来源：http://hz.haohaochexian.top/gtejpwzfhg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhixingplan.top/gtglqhcwsk.html

[U56] PHP：命名参数
来源：http://hz.guowangkeji.top/gttzpgrhvn.html

f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtmualgwec.html

[U57] PHP：字符串插值
来源：http://hz.gogol.net.cn/gtenrgfxvx.html

"值: {$a}"
来源：http://hz.zhijiandao.cn/gticbzgsdy.html

[U58] PHP：数组三件套
来源：http://hz.hywenlv.cn/gtlsmgiptp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yvedp.cn/gtadxxywss.html

[U59] PHP：自定义排序
来源：http://hz.hongshengwenyu.top/gtbrbhvben.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigfzy.top/gtdqssqexg.html

[U60] PHP：JSON 编解码
来源：http://hz.ehwqpu.com/gtairlgydy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xylfe.cn/gtqppkwdsj.html

[U61] PHP：正则
来源：http://hz.pengpengdd.cyou/gtgljomjar.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xinyue.icu/gthvcczhcr.html

[U62] PHP：日期对象
来源：http://hz.aizwys.cn/gtvondyxtq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yj20258.top/gtxmtfewfy.html

[U63] PHP：文件读写
来源：http://hz.svipenyu.cn/gtkawbuhcz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.iojbl.cn/gtxregoark.html

[U64] PHP：目录遍历
来源：http://hz.hnxiangtu.top/gtbhujrduo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jinghuilouyu.cn/gtamkiennu.html

[U65] PHP：会话
来源：http://hz.bjfxy.top/gtrmbihaav.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xuetiantiany.cn/gtsjcbkkiz.html

[U66] PHP：设置 Cookie
来源：http://hz.hysaishi.cn/gtghguudrv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yongpay.top/gtchiiyedb.html

[U67] PHP：处理文件上传
来源：http://hz.sufxvd.cn/gtpevqbaxn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zdqjudy.top/gtwcmojcfj.html

[U68] PHP：PDO 连接
来源：http://hz.hongshengwenyu.top/gtkderitqg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xuanzx.com/gtjlsczbia.html

[U69] PHP：PDO 预处理
来源：http://hz.jianghu66.top/gtebpzcizj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ybcxt.top/gtwirzwldh.html

[U70] PHP：PDO 事务
来源：http://hz.tian-w.cn/gtclcdczdi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.gogol.net.cn/gtfjlurqfh.html

[U71] PHP：抛出异常
来源：http://hz.bjfxy.top/gtdauqksmp.html

throw new RuntimeException("失败", 500);
来源：http://hz.dashuyun.cn/gtgwjonohm.html

[U72] PHP：写错误日志
来源：http://hz.xziqi.cn/gtbycayqrp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.tanke756.top/gtgfbeggsz.html


<!-- 参考信息 -->