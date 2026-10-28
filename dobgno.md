代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://hz.zhixingplan.top/gtrrolvrxe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xinyue.icu/gtrtxfrakn.html

[S48] C++：逐行读文件
来源：http://hz.c1oappe.top/gtimrnicun.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.meibo888.top/gtctggoyko.html

while (std::getline(in, line)) { }
来源：http://hz.ivvv.top/gtouxnofbi.html

[S49] C++：写文件
来源：http://hz.meibo888.top/gtpjqgihkx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ywan-chungtsiang.top/gtkukozbxm.html

[S50] C++：格式化数字
来源：http://hz.0kj1m.cn/gtxdgonjxe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jianghu66.top/gtgkuaxiis.html

[S51] C++：显式类型转换
来源：http://hz.jinghuilouyu.cn/gtcceozpgv.html

static_cast<double>(a) / b
来源：http://hz.jqgufenzy.top/gtbjhtlhet.html

[S52] C++：const 与 noexcept
来源：http://hz.xuanzx.com/gtzinhvwpp.html

int size() const noexcept { return n_; }
来源：http://hz.nwbrower.top/gtiyavqswd.html

[S53] C++：移动语义
来源：http://hz.ydjk.org.cn/gtiqbiojdn.html

std::vector<int> w = std::move(v);
来源：http://hz.zhaomingkeji.xyz/gtzukcihcz.html

[S54] C++：异常处理
来源：http://hz.yvedp.cn/gtnuscftag.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cheryme.top/gtbuysgqyi.html

[S55] C++：结构化绑定
来源：http://hz.yangfankeji.com/gtufamocfb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.feifeiyinyue.top/gturnvutuz.html

[S56] C++：optional
来源：http://hz.daxiang520.top/gtytcwtpnf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ywan-chungtsiang.top/gtkvizqtuq.html

[S57] C++：编译期常量
来源：http://hz.sweek.top/gtvktnfpxd.html

constexpr int N = 10;
来源：http://hz.zhijiandao.cn/gtshhuzghv.html

[S58] C++：命名空间
来源：http://hz.ybcxt.top/gtpynbhumi.html

namespace ns { int f() { return 1; } }
来源：http://hz.fzhhl.top/gtrvrnrtmr.html

[S59] C++：静态断言
来源：http://hz.jianghu66.top/gtfxzzmtmk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.dianchejie.cn/gtqkmtfzzc.html

[S60] C++：遍历并删除元素
来源：http://hz.ydjk.org.cn/gtexckotki.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jianghu66.top/gtxermpgld.html

================================================================================
来源：http://hz.chenzaomai.com/gtwjfcqbew.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.vqdsnc.cn/gtsbszxret.html

================================================================================
来源：http://hz.wangdashe.top/gtycvdflik.html

[T01] Kotlin：Hello World
来源：http://hz.ydzc1.top/gtwhlyydni.html

println("Hello")
来源：http://hz.hammf.cn/gtzritkmve.html

[T02] Kotlin：变量
来源：http://hz.gogol.net.cn/gtrbpnvlcc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinyuanbaomall.cn/gtyfdesyuz.html

[T03] Kotlin：字符串模板
来源：http://hz.zhaomingkeji.xyz/gtvqsrvble.html

"值: $b"
来源：http://hz.quarkkingdee.top/gtnooukjhb.html

[T04] Kotlin：空安全
来源：http://hz.kuanghao11.cn/gtaclhbgdv.html

val n: String? = null;  n?.length
来源：http://hz.xylfe.cn/gtsvxcupwa.html

[T05] Kotlin：when 表达式
来源：http://hz.fengsongda.top/gtsxcbulph.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.havefunace.top/gtoqguqjgh.html

[T06] Kotlin：集合映射
来源：http://hz.jinqigufen.top/gtcoeidbxx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hysaishi.cn/gtuiqkeawf.html

[T07] Kotlin：集合过滤
来源：http://hz.yuxming.cn/gtnajlvvnq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yonumen.top/gtfxbwjxzi.html

[T08] Kotlin：数据类
来源：http://hz.andypj.xyz/gtaujpltbm.html

data class User(val name: String, val age: Int)
来源：http://hz.zhiwuduotai.top/gtseguakje.html

[T09] Kotlin：扩展函数
来源：http://hz.cashguo.top/gteesjsguh.html

fun String.exclaim() = this + "!"
来源：http://hz.jqgufenzy.top/gtiwoghowi.html

[T10] Kotlin：默认参数
来源：http://hz.zhiwuduotai.top/gtanwstwdg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenzaomai.com/gtbybebnvy.html

[T11] Kotlin：协程
来源：http://hz.sweek.top/gtrurofkea.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zdqjudy.top/gtyzwvrzfb.html

[T12] Kotlin：解构声明
来源：http://hz.0kj1m.cn/gtprzawsdp.html

val (a, b) = Pair(1, 2)
来源：http://hz.xuetiantiany.cn/gtwiikhqdw.html

[T13] Kotlin：只读 Map
来源：http://hz.haohaochexian.top/gtfjbawcav.html

val m = mapOf("a" to 1)
来源：http://hz.tanke756.top/gtsuifbhme.html

[T14] Kotlin：循环
来源：http://hz.cdnleiting.top/gtqrbdqeuh.html

for (i in 1..10) println(i)
来源：http://hz.cucudq.cn/gtiokzdofh.html

[T15] Kotlin：接口
来源：http://hz.shuidangran.top/gtsfodvyts.html

interface Shape { fun area(): Double }
来源：http://hz.gotoacloud.top/gtutlftaek.html

[T16] Swift：Hello World
来源：http://hz.jlsjyb.cn/gtdusxifrr.html

print("Hello")
来源：http://hz.sufxvd.cn/gtduhwfqbi.html

[T17] Swift：变量与常量
来源：http://hz.sysykeji.top/gtjkvdwpdm.html

var a = 1;  let b = 2
来源：http://hz.wangdashe.top/gtqbcqeeub.html

[T18] Swift：字符串插值
来源：http://hz.hfpthk.cn/gtlwuqsnyg.html

"值: \(b)"
来源：http://hz.chenjidiqi.icu/gtbaqeecwg.html

[T19] Swift：可选绑定
来源：http://hz.shzxlz.cn/gtyexnankj.html

if let n = opt { print(n) }
来源：http://hz.9152youxi.cn/gtxjrqduif.html

[T20] Swift：数组操作
来源：http://hz.ydjk.org.cn/gtczrpfvke.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.0kj1m.cn/gturqpenzh.html

[T21] Swift：遍历
来源：http://hz.shangyingyoupin.top/gtihmxigxo.html

for x in a { print(x) }
来源：http://hz.xuetiantiany.cn/gtjpfgjclm.html

[T22] Swift：字典
来源：http://hz.ydjk.org.cn/gtedlzagzr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxuanxn.top/gtibcnchgd.html

[T23] Swift：函数
来源：http://hz.chenjidiqi.icu/gtmljscrli.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.svipenyu.cn/gtxiybtkzu.html

[T24] Swift：闭包
来源：http://hz.dashuyun.cn/gtkpuhhphu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jlsjyb.cn/gtyflyymok.html

[T25] Swift：结构体
来源：http://hz.cqqwz.cn/gtfacujwdf.html

struct P { var x: Int }
来源：http://hz.jqgfzy.top/gtpapuikwq.html

[T26] Swift：类与重写
来源：http://hz.yanxiufei.cn/gtfvzyheex.html

class A: Base { override func f() {} }
来源：http://hz.feifeiyinyue.top/gtdabguyda.html

[T27] Swift：错误处理
来源：http://hz.hnqzz.top/gtaofvaytg.html

do { try f() } catch { print(error) }
来源：http://hz.ywan-chungtsiang.top/gtkmdkabdj.html

[T28] Swift：枚举
来源：http://hz.chenjidiqi.icu/gtfasrhbth.html

enum Color { case red, green }
来源：http://hz.xingfuxueyuan.xyz/gtokwpxaxd.html

[T29] Swift：guard 提前返回
来源：http://hz.redwolf501.top/gtbztbxsdp.html

guard let x = opt else { return }
来源：http://hz.birdmap.top/gtkfgrmsoo.html

[T30] Swift：协议
来源：http://hz.meibo888.top/gtgwhjznfp.html

protocol Shape { func area() -> Double }
来源：http://hz.daxiang520.top/gtcczvzuos.html

[T31] Lua：Hello World
来源：http://hz.haohaochexian.top/gtxtginiir.html

print("Hello")
来源：http://hz.dashuyun.cn/gtzbzxxcjb.html

[T32] Lua：局部变量
来源：http://hz.cashguo.top/gtaacnttzt.html

local a = 1
来源：http://hz.andypj.xyz/gtcjlocgde.html

[T33] Lua：表（数组）
来源：http://hz.zhoulong.xyz/gtziukyjsw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cqqwz.cn/gtuhcniivt.html

[T34] Lua：遍历表
来源：http://hz.ppjwa.cn/gtwocgfyev.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hfpthk.cn/gtqztnpjpt.html

[T35] Lua：字典表
来源：http://hz.yj20258888.top/gtgsmgxmce.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xylfe.cn/gtaymwksrv.html

[T36] Lua：函数
来源：http://hz.jyoumei.cn/gttegfyicy.html

function add(a, b) return a + b end
来源：http://hz.hnxiangtu.top/gtyhifkozj.html

[T37] Lua：字符串拼接
来源：http://hz.yanxiufei.cn/gtkbtcfczk.html

"a" .. "b"
来源：http://hz.smart0.xyz/gtbvasluvw.html

[T38] Lua：条件
来源：http://hz.chenzaomai.com/gtnnxobfgg.html

if x > 0 then print("正") end
来源：http://hz.quarkkingdee.top/gtbvfytpex.html

[T39] Lua：模式匹配
来源：http://hz.yangfankeji.com/gtwsswhumg.html

string.find(s, "%d+")
来源：http://hz.jianghu66.top/gtgzdxdqgo.html

[T40] Lua：元表
来源：http://hz.yuxming.cn/gtcvaicowc.html

setmetatable({}, { __index = base })
来源：http://hz.chenlongwang.top/gtyyxhbzmd.html

[T41] Perl：Hello World
来源：http://hz.ppjwa.cn/gtpcuhbbya.html

print "Hello\n";
来源：http://hz.xuetiantiany.cn/gtxsprccku.html

[T42] Perl：变量类型
来源：http://hz.zycfv.cn/gtzfcwajvd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.52xcode.cn/gtbhosindk.html

[T43] Perl：字符串插值
来源：http://hz.hysaishi.cn/gtsmapmgfe.html

"值: $a"
来源：http://hz.zycfv.cn/gtbwkjykim.html

[T44] Perl：条件
来源：http://hz.xinyue.icu/gtngigosgm.html

if ($a > 0) { print "正"; }
来源：http://hz.yangfankeji.com/gtprnolhyt.html

[T45] Perl：数组遍历
来源：http://hz.feifeiyinyue.top/gtrincbkef.html

for my $x (@arr) { print $x; }
来源：http://hz.cucudq.cn/gtzuzwaujc.html

[T46] Perl：哈希操作
来源：http://hz.vqdsnc.cn/gtmdnlxrth.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.snrcjt.cn/gtugkntffa.html

[T47] Perl：正则捕获
来源：http://hz.fzhhl.top/gtjfqnqbmu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jqgfzy.top/gtiikxxudv.html

[T48] Perl：正则替换
来源：http://hz.haohaochexian.top/gtlemzqxcu.html

$s =~ s/old/new/g;
来源：http://hz.zhoulong.xyz/gtgbrrnsvu.html

[T49] Perl：函数
来源：http://hz.bjfxy.top/gtjiazyfaa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtzjaipjvk.html

[T50] Perl：逐行读文件
来源：http://hz.snrcjt.cn/gtliabbvmz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hongshengwenyu.top/gtcdfolilw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xuanzx.com/gtgxlommod.html

[T51] Scala：Hello World
来源：http://hz.hnxiangtu.top/gtjxfakhla.html

println("Hello")
来源：http://hz.jiagoushi.top/gtoplfhrns.html

[T52] Scala：变量
来源：http://hz.xuanzx.com/gtxveutjvd.html

val a = 1;  var b = 2
来源：http://hz.gogol.net.cn/gtnivkahjb.html

[T53] Scala：字符串插值
来源：http://hz.quarkkingdee.top/gtumrdtqwi.html

s"值: $b"
来源：http://hz.guannengcc.top/gtjryxuynb.html

[T54] Scala：集合映射
来源：http://hz.nwbrower.top/gtqjtbsppj.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.pycfn.com/gtshvoonpj.html

[T55] Scala：集合过滤
来源：http://hz.andypj.xyz/gtwscdmbox.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shuidangran.top/gthozderkj.html

[T56] Scala：样例类
来源：http://hz.9152youxi.cn/gtwoatguxn.html

case class User(name: String, age: Int)
来源：http://hz.svipenyu.cn/gtbhgmodwp.html

[T57] Scala：模式匹配
来源：http://hz.52xcode.cn/gtimdogooj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.c1oappe.top/gtgvkfqznv.html

[T58] Scala：函数定义
来源：http://hz.hnqzz.top/gtkktthqjc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.fzhhl.top/gtmpabmgzt.html

[T59] Scala：循环
来源：http://hz.havefunace.top/gtgdtyluvb.html

for (i <- 1 to 10) println(i)
来源：http://hz.yvedp.cn/gtwlooqyme.html

[T60] Scala：折叠
来源：http://hz.fzhhl.top/gthdjtcwfd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.guowangkeji.top/gtimyirrio.html

================================================================================
来源：http://hz.dashuyun.cn/gtbfvqthnx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hammf.cn/gtptpffuqq.html

================================================================================
来源：http://hz.cdnleiting.top/gtarboxmop.html

[U01] Py：创建虚拟环境
来源：http://hz.ppjwa.cn/gtpvcxrycz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zycfv.cn/gtrnsuexhm.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hongshengwenyu.top/gtpsabsrhw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xingfuxueyuan.xyz/gtggaofxeu.html

[U03] Py：加载 .env 配置
来源：http://hz.pycfn.com/gtaxreworr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.guowangkeji.top/gtrjxnjrxr.html

[U04] Py：变量调试打印
来源：http://hz.shanyushiyangtech.top/gtwkgnrzpc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhaomingkeji.xyz/gtvfwpywhi.html

[U05] Py：列表去重且保序
来源：http://hz.52xcode.cn/gtszkcbuox.html

list(dict.fromkeys(arr))
来源：http://hz.daxiang520.top/gtmxbzyqxl.html

[U06] Py：合并两个字典
来源：http://hz.yongpay.top/gtsgcqjzix.html

{**a, **b}
来源：http://hz.guowangkeji.top/gtmrfoarni.html

[U07] Py：反转字典键值
来源：http://hz.chenzaomai.com/gthiltbsjt.html

{v: k for k, v in d.items()}
来源：http://hz.xylfe.cn/gtutmgmmoj.html

[U08] Py：展平二维列表
来源：http://hz.pycfn.com/gtmbrcpooe.html

[y for x in nested for y in x]
来源：http://hz.jianghu66.top/gtptkhkzkv.html

[U09] Py：字典取最大值的键
来源：http://hz.xingfuxueyuan.xyz/gtoraihqqi.html

max(d, key=d.get)
来源：http://hz.tanke756.top/gtdudjnqwm.html

[U10] Py：按值排序字典
来源：http://hz.gotoacloud.top/gtadwhttfc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xziqi.cn/gtapnarwep.html

[U11] Py：生成器表达式
来源：http://hz.cqqwz.cn/gteapfllxr.html

(x * 2 for x in arr)
来源：http://hz.guowangkeji.top/gtwfmicmpy.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shangyingyoupin.top/gtfklslrmt.html

Counter(arr).most_common(3)
来源：http://hz.jinyuanbaomall.cn/gthuiponuu.html

[U13] Py：固定长度队列
来源：http://hz.wangshuangyany.cn/gtivetqtfs.html

deque(maxlen=10)
来源：http://hz.xylfe.cn/gthonnpluy.html

[U14] Py：分组收集到列表
来源：http://hz.nanxinkj.top/gtrfoaugyk.html

defaultdict(list)
来源：http://hz.sysykeji.top/gtprmgqwzv.html

[U15] Py：高精度计时
来源：http://hz.snrcjt.cn/gtqpnepqzv.html

t = time.perf_counter()
来源：http://hz.ydzc1.top/gtrjicgfyp.html

[U16] Py：命令行参数解析
来源：http://hz.sweek.top/gtjzywfdlc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.9152youxi.cn/gtqpbodqba.html

[U17] Py：初始化日志
来源：http://hz.cdnleiting.top/gthozxzgec.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhongyouzk.top/gtgmkitvni.html

[U18] Py：预编译正则
来源：http://hz.shanyushiyangtech.top/gttwbwkvzt.html

pat = re.compile(r"\d+")
来源：http://hz.gaohongyu789.top/gtldfhbkwh.html

[U19] Py：正则替换带回调
来源：http://hz.jqgufenzy.top/gtqkzogwak.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.svipenyu.cn/gtznjrrugw.html

[U20] Py：缓存函数结果
来源：http://hz.aizwys.cn/gtybrxeuey.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yanxiufei.cn/gtnmmfsvff.html

[U21] Py：自定义上下文管理器
来源：http://hz.ydjk.org.cn/gtnthdghin.html

@contextlib.contextmanager
来源：http://hz.aizwys.cn/gtsbskkkol.html

[U22] Py：矩阵转置
来源：http://hz.yangfankeji.com/gtmflaqxqo.html

list(zip(*m))
来源：http://hz.cashguo.top/gtfnpxfeht.html

[U23] Py：分块读取大文件
来源：http://hz.havefunace.top/gtzthdghdy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jqgfzy.top/gtegidxskz.html

[U24] Py：路径操作
来源：http://hz.sweek.top/gtziewgysf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xuanzx.com/gtbtgiejfh.html

[U25] Py：CSV 按字典读
来源：http://hz.cucudq.cn/gtzskkymqi.html

csv.DictReader(f)
来源：http://hz.shuidangran.top/gtoeryknlk.html

[U26] Py：并发下载
来源：http://hz.ivvv.top/gtvyzcgzfk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hysaishi.cn/gtvujtwovt.html

[U27] Py：异步 HTTP
来源：http://hz.chenzaomai.com/gtkejvkynz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sufxvd.cn/gtjecswnie.html

[U28] Py：类型别名
来源：http://hz.hongshengwenyu.top/gtqigzzots.html

UserId = int
来源：http://hz.jyoumei.cn/gtpjhpoomu.html

[U29] Py：属性校验
来源：http://hz.jinghuilouyu.cn/gtlrmvvfyo.html

@property 与 @x.setter 配合
来源：http://hz.hywenlv.cn/gtbyrjrmbv.html

[U30] Py：数据类
来源：http://hz.nanxuanxn.top/gtjunleodi.html

@dataclass(slots=True)
来源：http://hz.shzxlz.cn/gtptscrajf.html

[U31] Py：单测
来源：http://hz.xingfuxueyuan.xyz/gttojqhblu.html

python -m pytest -q
来源：http://hz.quarkkingdee.top/gtsxinfmdt.html

[U32] Py：代码格式化
来源：http://hz.yanxiufei.cn/gtbpqknewa.html

ruff format . && ruff check --fix .
来源：http://hz.ydzc1.top/gtwghhabvb.html

[U33] Py：打包发布
来源：http://hz.bjfxy.top/gtqtffvmkn.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hammf.cn/gtavvfvzbz.html

[U34] Py：判断编码
来源：http://hz.zhijiandao.cn/gtwhwsjlmo.html

chardet.detect(raw)
来源：http://hz.yvedp.cn/gtulrlizym.html

[U35] Py：发送邮件
来源：http://hz.yangfankeji.com/gtudfxukcp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jqgufenzy.top/gtfkvnmixl.html

[U36] Py：定时任务
来源：http://hz.cucudq.cn/gtzctisoal.html

schedule.every(10).minutes.do(job)
来源：http://hz.hywenlv.cn/gtfwudafsz.html

[U37] Py：读写 Excel
来源：http://hz.zhoulong.xyz/gtgwlbviog.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.redwolf501.top/gtwsaybhdf.html

[U38] Py：获取脚本所在目录
来源：http://hz.gogol.net.cn/gtoyanvcxo.html

Path(__file__).resolve().parent
来源：http://hz.jinqigfzy.top/gtjqpuiman.html

[U39] Py：判断是否在交互环境
来源：http://hz.jinyuanbaomall.cn/gtfnvdftpo.html

sys.stdout.isatty()
来源：http://hz.cucudq.cn/gtckeqqndl.html

[U40] Py：打印到标准错误
来源：http://hz.jinqigfzy.top/gtxccfiunq.html

print("err", file=sys.stderr)
来源：http://hz.gaohongyu789.top/gtbspjdqte.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ydzc1.top/gtptfiwped.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ybcxt.top/gtfrjovqmp.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yonumen.top/gtdyzfnpbr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yj20258.top/gtajfrdkvb.html

[U43] PHP：声明命名空间
来源：http://hz.jqgfzy.top/gthkktgwve.html

namespace App\Http;
来源：http://hz.chenzaomai.com/gtkzwjauha.html

[U44] PHP：开启严格类型
来源：http://hz.cqqwz.cn/gtapyflzwj.html

declare(strict_types=1);
来源：http://hz.wangdashe.top/gtlqasbgmx.html

[U45] PHP：类型声明与返回类型
来源：http://hz.aibaodan.cn/gtgigptups.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gtqkxhcwgs.html

[U46] PHP：可空类型
来源：http://hz.zhoulong.xyz/gtkvmaifam.html

?string $name = null
来源：http://hz.sufxvd.cn/gtydlrcihn.html

[U47] PHP：联合类型
来源：http://hz.316326.xyz/gtibdjjydr.html

int|string $id
来源：http://hz.jinqigufen.top/gtavqgkdmj.html

[U48] PHP：纯枚举
来源：http://hz.meibo888.top/gtokyridre.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zycfv.cn/gttorewdkl.html

[U49] PHP：只读属性
来源：http://hz.tianlin.xyz/gtainjzblx.html

public readonly string $name
来源：http://hz.hongshengwenyu.top/gtpzrbceeb.html

[U50] PHP：构造器属性提升
来源：http://hz.yj20258.top/gtmayufrfl.html

public function __construct(private int $id) {}
来源：http://hz.yj20258.top/gtnwjjbifo.html

[U51] PHP：数组解构
来源：http://hz.cqqwz.cn/gtzhzueeru.html

[$a, $b] = $arr;
来源：http://hz.xuetiantiany.cn/gtciegfzqh.html

[U52] PHP：箭头函数
来源：http://hz.zhongyouzk.top/gtkiwsedww.html

$double = fn($x) => $x * 2;
来源：http://hz.snrcjt.cn/gtomhqacwm.html

[U53] PHP：空合并运算符
来源：http://hz.hongshengwenyu.top/gtuxjtsheg.html

$v = $a ?? $b ?? "default";
来源：http://hz.0kj1m.cn/gtqkklbuyj.html

[U54] PHP：空安全调用
来源：http://hz.tian-w.cn/gtnbyfslej.html

$obj?->method()
来源：http://hz.jinyuanbaomall.cn/gtsbxhnbae.html

[U55] PHP：match 表达式
来源：http://hz.iojbl.cn/gttoazkcak.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hywenlv.cn/gtukrxcenn.html

[U56] PHP：命名参数
来源：http://hz.316326.xyz/gtyqtdaojw.html

f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtthoaeidp.html

[U57] PHP：字符串插值
来源：http://hz.hammf.cn/gtiayarchx.html

"值: {$a}"
来源：http://hz.haohaochexian.top/gtcdnlbstf.html

[U58] PHP：数组三件套
来源：http://hz.zdqjudy.top/gtharngrbw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xuanzx.com/gtdjmcnsph.html

[U59] PHP：自定义排序
来源：http://hz.cheryme.top/gtvfqyffqm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtutidxyia.html

[U60] PHP：JSON 编解码
来源：http://hz.fzhhl.top/gtbfxnpxou.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zdqjudy.top/gtsdjqsvgd.html

[U61] PHP：正则
来源：http://hz.daxiang520.top/gtuthctqjy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.guowangkeji.top/gtlfbishrf.html

[U62] PHP：日期对象
来源：http://hz.shuidangran.top/gtnjwrgbgb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cucudq.cn/gtbinurrvp.html

[U63] PHP：文件读写
来源：http://hz.zhoulong.xyz/gtgnhnkkfm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xuetiantiany.cn/gtbhxmudeg.html

[U64] PHP：目录遍历
来源：http://hz.cucudq.cn/gtcegwsmso.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.tanke756.top/gtfnhhxvcl.html

[U65] PHP：会话
来源：http://hz.nwbrower.top/gtguliafah.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.meibo888.top/gtmwntqscn.html

[U66] PHP：设置 Cookie
来源：http://hz.hammf.cn/gtmophkkrh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hongshengwenyu.top/gtxjxghmeo.html

[U67] PHP：处理文件上传
来源：http://hz.gotoacloud.top/gtvwhscydg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ybcxt.top/gtnwezgadh.html

[U68] PHP：PDO 连接
来源：http://hz.hammf.cn/gtlrooqcey.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yonumen.top/gtofozicwf.html

[U69] PHP：PDO 预处理
来源：http://hz.jyoumei.cn/gthcvuwqjh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cqqwz.cn/gttzygszki.html

[U70] PHP：PDO 事务
来源：http://hz.ppjwa.cn/gtfmzisiqz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.svipenyu.cn/gtdatvtpyh.html

[U71] PHP：抛出异常
来源：http://hz.vqdsnc.cn/gtzdjzkcwa.html

throw new RuntimeException("失败", 500);
来源：http://hz.yonumen.top/gtlosmcukg.html

[U72] PHP：写错误日志
来源：http://hz.yueranfly.top/gtpmdpiqem.html

error_log("失败: " . $e->getMessage());
来源：http://hz.wangdashe.top/gtxyuljhud.html


<!-- 参考信息 -->