代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://hz.shzxlz.cn/gtacbfbprt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgufenzy.top/gttuavaiiw.html

[S48] C++：逐行读文件
来源：http://hz.hywenlv.cn/gtwdqvbycr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shangyingyoupin.top/gtkqbmdogw.html

while (std::getline(in, line)) { }
来源：http://hz.cdnleiting.top/gttihyjjzv.html

[S49] C++：写文件
来源：http://hz.tian-w.cn/gtqsbpkdtp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.316326.xyz/gtyqqinqvp.html

[S50] C++：格式化数字
来源：http://hz.aizwys.cn/gtmvyncvwc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.guannengcc.top/gtbinobkpg.html

[S51] C++：显式类型转换
来源：http://hz.yonumen.top/gtsvmzrwar.html

static_cast<double>(a) / b
来源：http://hz.ivvv.top/gtdyeurkqk.html

[S52] C++：const 与 noexcept
来源：http://hz.ydjk.org.cn/gtfqchxsyd.html

int size() const noexcept { return n_; }
来源：http://hz.sxryk.cn/gtsjxzdhta.html

[S53] C++：移动语义
来源：http://hz.haohaochexian.top/gtgmhyzten.html

std::vector<int> w = std::move(v);
来源：http://hz.chenzaomai.com/gtpwngsnyx.html

[S54] C++：异常处理
来源：http://hz.52xcode.cn/gtgfpjuphv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shangyingyoupin.top/gtzixdxfgg.html

[S55] C++：结构化绑定
来源：http://hz.jyoumei.cn/gtsdefahrf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhaomingkeji.xyz/gtbwzzxbym.html

[S56] C++：optional
来源：http://hz.cqqwz.cn/gtqlgsyvvs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ydjk.org.cn/gtyrlczrta.html

[S57] C++：编译期常量
来源：http://hz.chenlongwang.top/gtzozrnequ.html

constexpr int N = 10;
来源：http://hz.ehwqpu.com/gtnovmfefu.html

[S58] C++：命名空间
来源：http://hz.cucudq.cn/gtkhdzyrow.html

namespace ns { int f() { return 1; } }
来源：http://hz.hnxiangtu.top/gtgfbmqign.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gtunwtkpfi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jlsjyb.cn/gtcmunrznk.html

[S60] C++：遍历并删除元素
来源：http://hz.jianghu66.top/gtlyfpiult.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shzxlz.cn/gttwwqkbvj.html

================================================================================
来源：http://hz.sxryk.cn/gtqxqhzskx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yangfankeji.com/gtlzkmvolb.html

================================================================================
来源：http://hz.tianlin.xyz/gtpvjgpzcd.html

[T01] Kotlin：Hello World
来源：http://hz.gzhubu.top/gtwvybcgui.html

println("Hello")
来源：http://hz.xziqi.cn/gtybqhdkfe.html

[T02] Kotlin：变量
来源：http://hz.zhoulong.xyz/gtimdfzush.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hysaishi.cn/gteejnwgcg.html

[T03] Kotlin：字符串模板
来源：http://hz.zhijiandao.cn/gtbasyrusk.html

"值: $b"
来源：http://hz.jyoumei.cn/gtafvcprnp.html

[T04] Kotlin：空安全
来源：http://hz.yj20258888.top/gtxqvqfski.html

val n: String? = null;  n?.length
来源：http://hz.zdqjudy.top/gttfiwyacm.html

[T05] Kotlin：when 表达式
来源：http://hz.jinyuanbaomall.cn/gtipxykzip.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gzhubu.top/gthwxiubct.html

[T06] Kotlin：集合映射
来源：http://hz.shanyushiyangkeji.top/gtnfalyggj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yvedp.cn/gtxshbmolt.html

[T07] Kotlin：集合过滤
来源：http://hz.shuidangran.top/gttqosfned.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.0kj1m.cn/gtztcapndq.html

[T08] Kotlin：数据类
来源：http://hz.zhoulong.xyz/gtvbfdmwqy.html

data class User(val name: String, val age: Int)
来源：http://hz.cucudq.cn/gtgqfuzyto.html

[T09] Kotlin：扩展函数
来源：http://hz.kuanghao11.cn/gtvhnwwfzy.html

fun String.exclaim() = this + "!"
来源：http://hz.jianghu66.top/gtbuvwmxif.html

[T10] Kotlin：默认参数
来源：http://hz.sufxvd.cn/gtrxrevsiz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yangfankeji.com/gtneuuruay.html

[T11] Kotlin：协程
来源：http://hz.dashuyun.cn/gtazsyzqov.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenzaomai.com/gtzhpnhvny.html

[T12] Kotlin：解构声明
来源：http://hz.wangdashe.top/gtrkxrkffw.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenlongwang.top/gtomxlwddk.html

[T13] Kotlin：只读 Map
来源：http://hz.dianchejie.cn/gtwmwbfmgk.html

val m = mapOf("a" to 1)
来源：http://hz.cashguo.top/gtdipqvuyp.html

[T14] Kotlin：循环
来源：http://hz.nwbrower.top/gtmvqudqfk.html

for (i in 1..10) println(i)
来源：http://hz.pycfn.com/gttdszjwjc.html

[T15] Kotlin：接口
来源：http://hz.jqgfzy.top/gthdjlacls.html

interface Shape { fun area(): Double }
来源：http://hz.wangshuangyany.cn/gtigixjlem.html

[T16] Swift：Hello World
来源：http://hz.nanxuanxn.top/gtpkizgdns.html

print("Hello")
来源：http://hz.jqgufenzy.top/gtqlhbfxat.html

[T17] Swift：变量与常量
来源：http://hz.yongpay.top/gthsckegtz.html

var a = 1;  let b = 2
来源：http://hz.316326.xyz/gtwedwgdkn.html

[T18] Swift：字符串插值
来源：http://hz.gaohongyu789.top/gtjlcwqixw.html

"值: \(b)"
来源：http://hz.fzhhl.top/gtkvwzwxru.html

[T19] Swift：可选绑定
来源：http://hz.tian-w.cn/gtpamvkqbs.html

if let n = opt { print(n) }
来源：http://hz.52xcode.cn/gtsxadleaz.html

[T20] Swift：数组操作
来源：http://hz.cqqwz.cn/gtxzbmribt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yanxiufei.cn/gtvpwvjphx.html

[T21] Swift：遍历
来源：http://hz.smart0.xyz/gtjobqbmum.html

for x in a { print(x) }
来源：http://hz.sufxvd.cn/gtyerbzzow.html

[T22] Swift：字典
来源：http://hz.xuetiantiany.cn/gtdsjaqgyl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.vqdsnc.cn/gtkwgyirer.html

[T23] Swift：函数
来源：http://hz.316326.xyz/gthlxfmfdj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nanxinkj.top/gtpwoqbfmm.html

[T24] Swift：闭包
来源：http://hz.kuanghao11.cn/gtrcaecpsr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ydzc1.top/gtucyjrmpf.html

[T25] Swift：结构体
来源：http://hz.hysaishi.cn/gttythpxbm.html

struct P { var x: Int }
来源：http://hz.hammf.cn/gtbjkblrrh.html

[T26] Swift：类与重写
来源：http://hz.shangyingyoupin.top/gtbxzpknyr.html

class A: Base { override func f() {} }
来源：http://hz.quarkkingdee.top/gtwldfglla.html

[T27] Swift：错误处理
来源：http://hz.birdmap.top/gtrcftrswq.html

do { try f() } catch { print(error) }
来源：http://hz.jyoumei.cn/gtajbgdsrc.html

[T28] Swift：枚举
来源：http://hz.gaohongyu789.top/gtsmhzuzcv.html

enum Color { case red, green }
来源：http://hz.ivvv.top/gtwsokruob.html

[T29] Swift：guard 提前返回
来源：http://hz.sufxvd.cn/gtpycjlenu.html

guard let x = opt else { return }
来源：http://hz.chenjidiqi.icu/gtapmhbbjp.html

[T30] Swift：协议
来源：http://hz.cashguo.top/gtczwihgdm.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigufen.top/gtzepahdly.html

[T31] Lua：Hello World
来源：http://hz.zhaomingkeji.xyz/gtrsmujxce.html

print("Hello")
来源：http://hz.guannengcc.top/gtuoiacjmt.html

[T32] Lua：局部变量
来源：http://hz.hongshengwenyu.top/gtdltsmrat.html

local a = 1
来源：http://hz.xinyue.icu/gtqxrvuqnu.html

[T33] Lua：表（数组）
来源：http://hz.hammf.cn/gticmfjqgq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jyoumei.cn/gttomiymnx.html

[T34] Lua：遍历表
来源：http://hz.tianlin.xyz/gtrzolzkbw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cqqwz.cn/gthgfbnzso.html

[T35] Lua：字典表
来源：http://hz.hnqzz.top/gtyaqxahau.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yongpay.top/gtytopwecw.html

[T36] Lua：函数
来源：http://hz.nwbrower.top/gtjajbbvre.html

function add(a, b) return a + b end
来源：http://hz.hnqzz.top/gtrzpiqxsv.html

[T37] Lua：字符串拼接
来源：http://hz.gzhubu.top/gtlfwyomxr.html

"a" .. "b"
来源：http://hz.cucudq.cn/gtbkxvswon.html

[T38] Lua：条件
来源：http://hz.sysykeji.top/gtrhdrulwv.html

if x > 0 then print("正") end
来源：http://hz.ydjk.org.cn/gtdmbizvri.html

[T39] Lua：模式匹配
来源：http://hz.yuanzhike.top/gteekinkcv.html

string.find(s, "%d+")
来源：http://hz.sufxvd.cn/gtxakovqgx.html

[T40] Lua：元表
来源：http://hz.fengsongda.top/gtbrlppbmv.html

setmetatable({}, { __index = base })
来源：http://hz.chenjidiqi.icu/gtguvrrynm.html

[T41] Perl：Hello World
来源：http://hz.fengsongda.top/gtunvbndcd.html

print "Hello\n";
来源：http://hz.xuanzx.com/gtuzezixoq.html

[T42] Perl：变量类型
来源：http://hz.zhoulong.xyz/gtqwcomxac.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinqigfzy.top/gtodtdlecp.html

[T43] Perl：字符串插值
来源：http://hz.shangyingyoupin.top/gtfvjwlavi.html

"值: $a"
来源：http://hz.zycfv.cn/gtxsmyypmo.html

[T44] Perl：条件
来源：http://hz.kuanghao11.cn/gtitufqsab.html

if ($a > 0) { print "正"; }
来源：http://hz.nwbrower.top/gthliramrc.html

[T45] Perl：数组遍历
来源：http://hz.xuanzx.com/gtdusaqheu.html

for my $x (@arr) { print $x; }
来源：http://hz.nwbrower.top/gtocthczum.html

[T46] Perl：哈希操作
来源：http://hz.kuanghao11.cn/gtespojzbu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hongshengwenyu.top/gtgwzyaaub.html

[T47] Perl：正则捕获
来源：http://hz.jiagoushi.top/gtzbimlple.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhiwuduotai.top/gtbhvmefql.html

[T48] Perl：正则替换
来源：http://hz.snrcjt.cn/gtblrglrbs.html

$s =~ s/old/new/g;
来源：http://hz.nwbrower.top/gtwvjolith.html

[T49] Perl：函数
来源：http://hz.daxiang520.top/gtkuprzwyf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.dashuyun.cn/gtelduthdv.html

[T50] Perl：逐行读文件
来源：http://hz.wangshuangyany.cn/gtxcqsczid.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenjidiqi.icu/gtheofglla.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinqigfzy.top/gtouurlsmi.html

[T51] Scala：Hello World
来源：http://hz.xuanzx.com/gtoryjsyoq.html

println("Hello")
来源：http://hz.zhongyouzk.top/gtmaqhszud.html

[T52] Scala：变量
来源：http://hz.sufxvd.cn/gtmysqggvc.html

val a = 1;  var b = 2
来源：http://hz.jyoumei.cn/gtvhwrrcrj.html

[T53] Scala：字符串插值
来源：http://hz.redwolf501.top/gtdyuzfkgw.html

s"值: $b"
来源：http://hz.wangshuangyany.cn/gtrfvfvhdp.html

[T54] Scala：集合映射
来源：http://hz.zdqjudy.top/gtzczvwebd.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.meibo888.top/gtovnvapsy.html

[T55] Scala：集合过滤
来源：http://hz.tian-w.cn/gtswmgvoze.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.andypj.xyz/gtzpfstimc.html

[T56] Scala：样例类
来源：http://hz.aibaodan.cn/gtplouvfjk.html

case class User(name: String, age: Int)
来源：http://hz.aizwys.cn/gtiqjiaebh.html

[T57] Scala：模式匹配
来源：http://hz.jinqigfzy.top/gtbucaufae.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinqigufen.top/gtdlmoxdxw.html

[T58] Scala：函数定义
来源：http://hz.jianghu66.top/gttnfecwyz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.316326.xyz/gtabqfcuru.html

[T59] Scala：循环
来源：http://hz.xuetiantiany.cn/gtgcatblef.html

for (i <- 1 to 10) println(i)
来源：http://hz.nwbrower.top/gtsazjigsh.html

[T60] Scala：折叠
来源：http://hz.aibaodan.cn/gtyprhlfki.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xinyue.icu/gtarrmkudn.html

================================================================================
来源：http://hz.aizwys.cn/gtoojaholb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gaohongyu789.top/gtjoopqoiv.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtkrkwpdzm.html

[U01] Py：创建虚拟环境
来源：http://hz.svipenyu.cn/gtvovnqjgl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhijiandao.cn/gtpmgfksgv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.smart0.xyz/gtvazqawkr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.nwbrower.top/gtkcpszlem.html

[U03] Py：加载 .env 配置
来源：http://hz.iojbl.cn/gthqzmdlge.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.nanxuanxn.top/gtiohhfsqg.html

[U04] Py：变量调试打印
来源：http://hz.redwolf501.top/gtwcweqeld.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinghuilouyu.cn/gtqxbdwplc.html

[U05] Py：列表去重且保序
来源：http://hz.feifeiyinyue.top/gtukpukayq.html

list(dict.fromkeys(arr))
来源：http://hz.yongpay.top/gtjgcjxoml.html

[U06] Py：合并两个字典
来源：http://hz.yuxming.cn/gtgyyhybnc.html

{**a, **b}
来源：http://hz.dianchejie.cn/gttadppjsr.html

[U07] Py：反转字典键值
来源：http://hz.9152youxi.cn/gtflfbxrhx.html

{v: k for k, v in d.items()}
来源：http://hz.yuanzhike.top/gtwqecotml.html

[U08] Py：展平二维列表
来源：http://hz.xylfe.cn/gtaxtlnuzr.html

[y for x in nested for y in x]
来源：http://hz.wangshuangyany.cn/gtpsqibmis.html

[U09] Py：字典取最大值的键
来源：http://hz.daria6918.cn/gtxhkxxkxs.html

max(d, key=d.get)
来源：http://hz.yuxming.cn/gtllfaujgg.html

[U10] Py：按值排序字典
来源：http://hz.zhongyouzk.top/gtbbchxmqj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.wangdashe.top/gtddshnqea.html

[U11] Py：生成器表达式
来源：http://hz.daria6918.cn/gtglfqhimu.html

(x * 2 for x in arr)
来源：http://hz.xuanzx.com/gtmjorosjj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yonumen.top/gtrztpmemq.html

Counter(arr).most_common(3)
来源：http://hz.jlsjyb.cn/gtgevstfzk.html

[U13] Py：固定长度队列
来源：http://hz.hfpthk.cn/gtygnifenf.html

deque(maxlen=10)
来源：http://hz.xuanzx.com/gtfmpnpguf.html

[U14] Py：分组收集到列表
来源：http://hz.cucudq.cn/gtqrrtjtgr.html

defaultdict(list)
来源：http://hz.guannengcc.top/gtefinnstt.html

[U15] Py：高精度计时
来源：http://hz.nanxinkj.top/gtnpkntszs.html

t = time.perf_counter()
来源：http://hz.hammf.cn/gtmgkmxhal.html

[U16] Py：命令行参数解析
来源：http://hz.feifeiyinyue.top/gtqhogbmpb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhengqikj.top/gtariagzkj.html

[U17] Py：初始化日志
来源：http://hz.xylfe.cn/gtuqhgpplb.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.haohaochexian.top/gtoxapxank.html

[U18] Py：预编译正则
来源：http://hz.zhongyouzk.top/gtabqldtlp.html

pat = re.compile(r"\d+")
来源：http://hz.andypj.xyz/gtdusscqyv.html

[U19] Py：正则替换带回调
来源：http://hz.yonumen.top/gtmmywtnso.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sufxvd.cn/gtmwgvobls.html

[U20] Py：缓存函数结果
来源：http://hz.xuanzx.com/gtapuvvegt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shangyingyoupin.top/gtbvhoegqu.html

[U21] Py：自定义上下文管理器
来源：http://hz.zycfv.cn/gtmyhkgosh.html

@contextlib.contextmanager
来源：http://hz.xingfuxueyuan.xyz/gtgeamnvme.html

[U22] Py：矩阵转置
来源：http://hz.nanxinkj.top/gtmqxities.html

list(zip(*m))
来源：http://hz.gogol.net.cn/gtftxlzhdv.html

[U23] Py：分块读取大文件
来源：http://hz.wangshuangyany.cn/gtnqiqvouv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.meibo888.top/gtukekvldn.html

[U24] Py：路径操作
来源：http://hz.jiagoushi.top/gtwhmadqlv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhongyouzk.top/gtxsivkoix.html

[U25] Py：CSV 按字典读
来源：http://hz.cashguo.top/gtpexwaztr.html

csv.DictReader(f)
来源：http://hz.shzxlz.cn/gtanqxhmpy.html

[U26] Py：并发下载
来源：http://hz.gogol.net.cn/gtyaoqhlos.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.guannengcc.top/gtgsfrkbyq.html

[U27] Py：异步 HTTP
来源：http://hz.svipenyu.cn/gtqqcbrekn.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.bjfxy.top/gtbcwbjkju.html

[U28] Py：类型别名
来源：http://hz.gaohongyu789.top/gtzwwjhjnj.html

UserId = int
来源：http://hz.yuxming.cn/gtjizwbedv.html

[U29] Py：属性校验
来源：http://hz.yanxiufei.cn/gtmlfxlfke.html

@property 与 @x.setter 配合
来源：http://hz.chenlongwang.top/gtuwijhexx.html

[U30] Py：数据类
来源：http://hz.shuidangran.top/gtysxeiycb.html

@dataclass(slots=True)
来源：http://hz.cashguo.top/gtvraqddjs.html

[U31] Py：单测
来源：http://hz.yvedp.cn/gtycpasont.html

python -m pytest -q
来源：http://hz.wangshuangyany.cn/gthdfwunbk.html

[U32] Py：代码格式化
来源：http://hz.sysykeji.top/gtgytqnbxh.html

ruff format . && ruff check --fix .
来源：http://hz.chenlongwang.top/gtajjtdqnz.html

[U33] Py：打包发布
来源：http://hz.kuanghao11.cn/gthuzavxte.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xuanzx.com/gterwuzqwa.html

[U34] Py：判断编码
来源：http://hz.cheryme.top/gtrqtksirr.html

chardet.detect(raw)
来源：http://hz.zycfv.cn/gtwnjggepp.html

[U35] Py：发送邮件
来源：http://hz.iojbl.cn/gtmbhsbvcy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.fengsongda.top/gtbvtbfaer.html

[U36] Py：定时任务
来源：http://hz.yanxiufei.cn/gtmukmmtji.html

schedule.every(10).minutes.do(job)
来源：http://hz.shangyingyoupin.top/gtyckpoglj.html

[U37] Py：读写 Excel
来源：http://hz.jinyuanbaomall.cn/gtyrivilbx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.aibaodan.cn/gtlufaizhn.html

[U38] Py：获取脚本所在目录
来源：http://hz.redwolf501.top/gtrioxejyb.html

Path(__file__).resolve().parent
来源：http://hz.gaohongyu789.top/gtgwqmfrqk.html

[U39] Py：判断是否在交互环境
来源：http://hz.hammf.cn/gthjmvbwfm.html

sys.stdout.isatty()
来源：http://hz.jianghu66.top/gtuzvfpceg.html

[U40] Py：打印到标准错误
来源：http://hz.wangdashe.top/gtowvpsfuc.html

print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtyynunmlo.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ybcxt.top/gtifkwkwov.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xingfuxueyuan.xyz/gtjrvasmbp.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.havefunace.top/gtteznqhlq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.316326.xyz/gtuszstjiq.html

[U43] PHP：声明命名空间
来源：http://hz.zycfv.cn/gtljfsfqsl.html

namespace App\Http;
来源：http://hz.ppjwa.cn/gtevutgpqa.html

[U44] PHP：开启严格类型
来源：http://hz.xinyue.icu/gtrgqtddtx.html

declare(strict_types=1);
来源：http://hz.hywenlv.cn/gtqahpqfiw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.tianlin.xyz/gtcrskniuc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtjryzoiee.html

[U46] PHP：可空类型
来源：http://hz.cucudq.cn/gtstumhatd.html

?string $name = null
来源：http://hz.iojbl.cn/gtklrwmqro.html

[U47] PHP：联合类型
来源：http://hz.sysykeji.top/gtxhikylan.html

int|string $id
来源：http://hz.zhengqikj.top/gtmrwcryqu.html

[U48] PHP：纯枚举
来源：http://hz.jlsjyb.cn/gtmauzaxyo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinqigfzy.top/gtwjvoihmx.html

[U49] PHP：只读属性
来源：http://hz.haohaochexian.top/gtdbusabbw.html

public readonly string $name
来源：http://hz.xziqi.cn/gtuikaybes.html

[U50] PHP：构造器属性提升
来源：http://hz.mhx1999.top/gtqkarwyoc.html

public function __construct(private int $id) {}
来源：http://hz.havefunace.top/gttlalxbrd.html

[U51] PHP：数组解构
来源：http://hz.tian-w.cn/gtvmiekfxg.html

[$a, $b] = $arr;
来源：http://hz.jinqigfzy.top/gtumwxeqtw.html

[U52] PHP：箭头函数
来源：http://hz.shanyushiyangkeji.top/gttjxhhbus.html

$double = fn($x) => $x * 2;
来源：http://hz.birdmap.top/gtyiojdfud.html

[U53] PHP：空合并运算符
来源：http://hz.hnqzz.top/gtwfbehngn.html

$v = $a ?? $b ?? "default";
来源：http://hz.xziqi.cn/gtfvpurtiz.html

[U54] PHP：空安全调用
来源：http://hz.zhoulong.xyz/gtmblmebif.html

$obj?->method()
来源：http://hz.zhijiandao.cn/gtlspigxsv.html

[U55] PHP：match 表达式
来源：http://hz.yj20258888.top/gtnilclkxf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sysykeji.top/gtxkicnavd.html

[U56] PHP：命名参数
来源：http://hz.shangyingyoupin.top/gtmmenvhnp.html

f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtdjdbtonv.html

[U57] PHP：字符串插值
来源：http://hz.9152youxi.cn/gtozqdatoz.html

"值: {$a}"
来源：http://hz.yj202588.top/gtpvofvpfl.html

[U58] PHP：数组三件套
来源：http://hz.zhengqikj.top/gtcvgbztnq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.haohaochexian.top/gtsdvdxscd.html

[U59] PHP：自定义排序
来源：http://hz.redwolf501.top/gtpaijfstj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xylfe.cn/gtdqnlcbnj.html

[U60] PHP：JSON 编解码
来源：http://hz.hysaishi.cn/gtmdwknyda.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.feifeiyinyue.top/gtjbuaavrk.html

[U61] PHP：正则
来源：http://hz.tanke756.top/gtzbigoqwv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cheryme.top/gtlofakior.html

[U62] PHP：日期对象
来源：http://hz.sufxvd.cn/gtprrjetbz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.guowangkeji.top/gtnvgkvujc.html

[U63] PHP：文件读写
来源：http://hz.ivvv.top/gttrynhsiu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.c1oappe.top/gtzayxwbru.html

[U64] PHP：目录遍历
来源：http://hz.feifeiyinyue.top/gtbxayncyc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yuxming.cn/gtqtqmcunz.html

[U65] PHP：会话
来源：http://hz.yongpay.top/gttxivfpjt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.aizwys.cn/gthrzqholh.html

[U66] PHP：设置 Cookie
来源：http://hz.bjfxy.top/gtbbjxryjy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.fengsongda.top/gtjtgmqqxk.html

[U67] PHP：处理文件上传
来源：http://hz.pycfn.com/gtcwextxex.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.cqqwz.cn/gtamgsljsy.html

[U68] PHP：PDO 连接
来源：http://hz.zhixingplan.top/gtjfsgagxs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cqqwz.cn/gtstphgrau.html

[U69] PHP：PDO 预处理
来源：http://hz.quarkkingdee.top/gtsvwknwey.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.shzxlz.cn/gtkxcmagnh.html

[U70] PHP：PDO 事务
来源：http://hz.hammf.cn/gtatuyynmr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cashguo.top/gtacgooolu.html

[U71] PHP：抛出异常
来源：http://hz.shanyushiyangkeji.top/gtsdbpziuc.html

throw new RuntimeException("失败", 500);
来源：http://hz.snrcjt.cn/gtfrpqzgfs.html

[U72] PHP：写错误日志
来源：http://hz.bjfxy.top/gthbzptumt.html

error_log("失败: " . $e->getMessage());
来源：http://hz.bjfxy.top/gtuujnfsez.html


<!-- 参考信息 -->