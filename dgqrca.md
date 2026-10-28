代发 wailian999

[S39] C++：自定义比较器排序
来源：http://hz.zhongyouzk.top/gtwogslowd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cucudq.cn/gtkqhaxbzn.html

[S40] C++：查找元素
来源：http://hz.c1oappe.top/gtlnssyane.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guannengcc.top/gttbqzbaqx.html

[S41] C++：类与构造函数
来源：http://hz.shanyushiyangtech.top/gtgtcckgar.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.svipenyu.cn/gtaqkmbthj.html

[S42] C++：继承与虚函数
来源：http://hz.hongshengwenyu.top/gtbbzrzhnc.html

class B : public Base { public: void f() override {} };
来源：http://hz.yuxming.cn/gtvwkxdyym.html

[S43] C++：智能指针
来源：http://hz.zhixingplan.top/gtnijrubsc.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxinkj.top/gthpezmoss.html

[S44] C++：引用传参
来源：http://hz.daxiang520.top/gtugcjqeak.html

void inc(int &x) { ++x; }
来源：http://hz.xinyue.icu/gtseryltkv.html

[S45] C++：lambda
来源：http://hz.gzhubu.top/gtkdzoutwc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cdnleiting.top/gtzcdnfsrr.html

[S46] C++：函数模板
来源：http://hz.gzhubu.top/gtzpdwrvyi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhijiandao.cn/gthjlgqruq.html

[S47] C++：结构化绑定遍历
来源：http://hz.ivvv.top/gtfovoaian.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.9152youxi.cn/gtkoreyvsz.html

[S48] C++：逐行读文件
来源：http://hz.shzxlz.cn/gtqjatpcgy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.haohaochexian.top/gtervledkg.html

while (std::getline(in, line)) { }
来源：http://hz.yongpay.top/gtjzjmjwhr.html

[S49] C++：写文件
来源：http://hz.haohaochexian.top/gtayhoqoxx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinqigufen.top/gtdtsmhlfa.html

[S50] C++：格式化数字
来源：http://hz.yonumen.top/gtuelkzmbs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daria6918.cn/gtoumndyrn.html

[S51] C++：显式类型转换
来源：http://hz.zhongyouzk.top/gtymmrdlge.html

static_cast<double>(a) / b
来源：http://hz.feifeiyinyue.top/gtgkotvceu.html

[S52] C++：const 与 noexcept
来源：http://hz.jyoumei.cn/gtoycwvyqm.html

int size() const noexcept { return n_; }
来源：http://hz.haohaochexian.top/gturqfsbse.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gthtuvvjgx.html

std::vector<int> w = std::move(v);
来源：http://hz.hammf.cn/gtzkwnswog.html

[S54] C++：异常处理
来源：http://hz.yvedp.cn/gtksbnnlgd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.mhx1999.top/gtrxbxcpye.html

[S55] C++：结构化绑定
来源：http://hz.chenjidiqi.icu/gthdcvvrtw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aibaodan.cn/gtlsdesewv.html

[S56] C++：optional
来源：http://hz.fzhhl.top/gtbeidtmul.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.pengpengdd.cyou/gtoeaajubr.html

[S57] C++：编译期常量
来源：http://hz.hfpthk.cn/gtzcrgzonu.html

constexpr int N = 10;
来源：http://hz.yangfankeji.com/gtzechubfc.html

[S58] C++：命名空间
来源：http://hz.nanxuanxn.top/gtkwvcjdio.html

namespace ns { int f() { return 1; } }
来源：http://hz.yuanzhike.top/gtfszpvnul.html

[S59] C++：静态断言
来源：http://hz.chenzaomai.com/gtcxosioeb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hnxiangtu.top/gtiildpiut.html

[S60] C++：遍历并删除元素
来源：http://hz.gaohongyu789.top/gtqqlpxmpc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gotoacloud.top/gtokaecscp.html

================================================================================
来源：http://hz.gzhubu.top/gtejmhmmiu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.havefunace.top/gtunupxllo.html

================================================================================
来源：http://hz.yangfankeji.com/gtucrrlejb.html

[T01] Kotlin：Hello World
来源：http://hz.sxryk.cn/gtbkjnhtsk.html

println("Hello")
来源：http://hz.dianchejie.cn/gtbbbpiemt.html

[T02] Kotlin：变量
来源：http://hz.yj20258.top/gtfzbfmgqz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.andypj.xyz/gtbsbwhfyw.html

[T03] Kotlin：字符串模板
来源：http://hz.zhiwuduotai.top/gtnukmhssb.html

"值: $b"
来源：http://hz.daria6918.cn/gtrglvjzie.html

[T04] Kotlin：空安全
来源：http://hz.yj20258888.top/gtdrxzvmbl.html

val n: String? = null;  n?.length
来源：http://hz.pengpengdd.cyou/gtoxdtpfhy.html

[T05] Kotlin：when 表达式
来源：http://hz.ppjwa.cn/gtdgyqbhkf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xinyue.icu/gtsamytlsk.html

[T06] Kotlin：集合映射
来源：http://hz.yangfankeji.com/gtdhfqmwbx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shzxlz.cn/gtqwakeocg.html

[T07] Kotlin：集合过滤
来源：http://hz.zdqjudy.top/gtovhdgfje.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xingfuxueyuan.xyz/gtddligagp.html

[T08] Kotlin：数据类
来源：http://hz.meibo888.top/gtxomtrxfg.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgufenzy.top/gtsmyzlccn.html

[T09] Kotlin：扩展函数
来源：http://hz.nwbrower.top/gtcpczvdww.html

fun String.exclaim() = this + "!"
来源：http://hz.jinqigufen.top/gtwrymcvmw.html

[T10] Kotlin：默认参数
来源：http://hz.cheryme.top/gtdujecyxp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.smart0.xyz/gtujjhjinv.html

[T11] Kotlin：协程
来源：http://hz.quarkkingdee.top/gtgjfyxeoi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigfzy.top/gtzwkxplak.html

[T12] Kotlin：解构声明
来源：http://hz.pycfn.com/gtutdeyzzx.html

val (a, b) = Pair(1, 2)
来源：http://hz.xylfe.cn/gtwxzvmzvu.html

[T13] Kotlin：只读 Map
来源：http://hz.tianlin.xyz/gtbsxurkte.html

val m = mapOf("a" to 1)
来源：http://hz.andypj.xyz/gtlvfdqcbn.html

[T14] Kotlin：循环
来源：http://hz.pengpengdd.cyou/gtqhnaufxp.html

for (i in 1..10) println(i)
来源：http://hz.zhiwuduotai.top/gtarglgprg.html

[T15] Kotlin：接口
来源：http://hz.gotoacloud.top/gtxpdnmoxk.html

interface Shape { fun area(): Double }
来源：http://hz.hammf.cn/gtkkycpije.html

[T16] Swift：Hello World
来源：http://hz.yj202588.top/gtnxyzvfiv.html

print("Hello")
来源：http://hz.havefunace.top/gthzwlnleu.html

[T17] Swift：变量与常量
来源：http://hz.yangfankeji.com/gtxxunkzni.html

var a = 1;  let b = 2
来源：http://hz.sufxvd.cn/gthenlhhqu.html

[T18] Swift：字符串插值
来源：http://hz.jqgfzy.top/gtmbdwhyql.html

"值: \(b)"
来源：http://hz.shanyushiyangtech.top/gtswgwsoth.html

[T19] Swift：可选绑定
来源：http://hz.xylfe.cn/gtskskhagy.html

if let n = opt { print(n) }
来源：http://hz.pengpengdd.cyou/gtdfsekfdk.html

[T20] Swift：数组操作
来源：http://hz.aibaodan.cn/gtvbomgggs.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhijiandao.cn/gteaigsnjc.html

[T21] Swift：遍历
来源：http://hz.jqgufenzy.top/gtidxdhxfa.html

for x in a { print(x) }
来源：http://hz.ydjk.org.cn/gtdutjmzjp.html

[T22] Swift：字典
来源：http://hz.yueranfly.top/gtmxqqgpjj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.quarkkingdee.top/gtpjqiwsjj.html

[T23] Swift：函数
来源：http://hz.jlsjyb.cn/gtwqwqsnwi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.pycfn.com/gtktbnvyol.html

[T24] Swift：闭包
来源：http://hz.nanxuanxn.top/gtnztvqzlt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhengqikj.top/gtvdbbodkz.html

[T25] Swift：结构体
来源：http://hz.hammf.cn/gtkawtweae.html

struct P { var x: Int }
来源：http://hz.hammf.cn/gtixkejobp.html

[T26] Swift：类与重写
来源：http://hz.zhiwuduotai.top/gttsuducos.html

class A: Base { override func f() {} }
来源：http://hz.9152youxi.cn/gtcbizvwms.html

[T27] Swift：错误处理
来源：http://hz.gogol.net.cn/gtleprajfw.html

do { try f() } catch { print(error) }
来源：http://hz.cucudq.cn/gtptgdlxtg.html

[T28] Swift：枚举
来源：http://hz.jqgufenzy.top/gtptngrbpi.html

enum Color { case red, green }
来源：http://hz.yj202588.top/gtnvvuejeo.html

[T29] Swift：guard 提前返回
来源：http://hz.ehwqpu.com/gtkvgidmos.html

guard let x = opt else { return }
来源：http://hz.zhengqikj.top/gtgfwalogf.html

[T30] Swift：协议
来源：http://hz.cashguo.top/gtdektoowc.html

protocol Shape { func area() -> Double }
来源：http://hz.quarkkingdee.top/gtddrphtys.html

[T31] Lua：Hello World
来源：http://hz.jinqigfzy.top/gtiyiiwzzo.html

print("Hello")
来源：http://hz.gotoacloud.top/gtmkjrqxee.html

[T32] Lua：局部变量
来源：http://hz.mhx1999.top/gtnsrzvofr.html

local a = 1
来源：http://hz.dashuyun.cn/gtaqjnbelt.html

[T33] Lua：表（数组）
来源：http://hz.yangfankeji.com/gtwabnvovs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.c1oappe.top/gtystezqtf.html

[T34] Lua：遍历表
来源：http://hz.cdnleiting.top/gtylpoffeq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ywan-chungtsiang.top/gtvqnriowl.html

[T35] Lua：字典表
来源：http://hz.nwbrower.top/gtxpsovewr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yonumen.top/gtvarxozlf.html

[T36] Lua：函数
来源：http://hz.hnxiangtu.top/gtaloviyah.html

function add(a, b) return a + b end
来源：http://hz.chenjidiqi.icu/gtkeldppkx.html

[T37] Lua：字符串拼接
来源：http://hz.meibo888.top/gtqpithobd.html

"a" .. "b"
来源：http://hz.jqgfzy.top/gthgprglnp.html

[T38] Lua：条件
来源：http://hz.c1oappe.top/gtzsxagwau.html

if x > 0 then print("正") end
来源：http://hz.zycfv.cn/gtewufztjg.html

[T39] Lua：模式匹配
来源：http://hz.cashguo.top/gtckzhqowr.html

string.find(s, "%d+")
来源：http://hz.ywan-chungtsiang.top/gtxdiirggk.html

[T40] Lua：元表
来源：http://hz.yvedp.cn/gtavksmwrz.html

setmetatable({}, { __index = base })
来源：http://hz.shanyushiyangtech.top/gtqwewpagi.html

[T41] Perl：Hello World
来源：http://hz.fengsongda.top/gtdxadywfj.html

print "Hello\n";
来源：http://hz.xziqi.cn/gtrpfosepw.html

[T42] Perl：变量类型
来源：http://hz.sufxvd.cn/gtufzmvxbt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.dashuyun.cn/gtbicxpvjd.html

[T43] Perl：字符串插值
来源：http://hz.316326.xyz/gtpclmvdad.html

"值: $a"
来源：http://hz.daria6918.cn/gtwllbgrhl.html

[T44] Perl：条件
来源：http://hz.tian-w.cn/gtiweeutae.html

if ($a > 0) { print "正"; }
来源：http://hz.feifeiyinyue.top/gtnepqxekv.html

[T45] Perl：数组遍历
来源：http://hz.pycfn.com/gtvhoeqfgd.html

for my $x (@arr) { print $x; }
来源：http://hz.shuidangran.top/gtehlnrwsp.html

[T46] Perl：哈希操作
来源：http://hz.gzhubu.top/gtiikdopsd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xinyue.icu/gtvexafqzf.html

[T47] Perl：正则捕获
来源：http://hz.0kj1m.cn/gtsohtdyrl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sweek.top/gtulaatxjt.html

[T48] Perl：正则替换
来源：http://hz.sufxvd.cn/gtsuvjcmwb.html

$s =~ s/old/new/g;
来源：http://hz.fengsongda.top/gtvobyllnc.html

[T49] Perl：函数
来源：http://hz.0kj1m.cn/gtlbdlagsr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.andypj.xyz/gtxeorjvsl.html

[T50] Perl：逐行读文件
来源：http://hz.sufxvd.cn/gtvegvyqlh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.daxiang520.top/gtkpicrkfj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.smart0.xyz/gtxvmjsqdi.html

[T51] Scala：Hello World
来源：http://hz.ehwqpu.com/gttjuwphqi.html

println("Hello")
来源：http://hz.vqdsnc.cn/gtzlswjbau.html

[T52] Scala：变量
来源：http://hz.smart0.xyz/gtmzxloknz.html

val a = 1;  var b = 2
来源：http://hz.zhixingplan.top/gtzwgeqiwp.html

[T53] Scala：字符串插值
来源：http://hz.9152youxi.cn/gtfytdukka.html

s"值: $b"
来源：http://hz.mhx1999.top/gtlmwnnztw.html

[T54] Scala：集合映射
来源：http://hz.jiagoushi.top/gtthitbpmt.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.feifeiyinyue.top/gtprckamth.html

[T55] Scala：集合过滤
来源：http://hz.jinqigfzy.top/gtucqjegzp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sysykeji.top/gtkutyppwx.html

[T56] Scala：样例类
来源：http://hz.ydjk.org.cn/gtryedxtli.html

case class User(name: String, age: Int)
来源：http://hz.hfpthk.cn/gtflpjlrqr.html

[T57] Scala：模式匹配
来源：http://hz.ivvv.top/gtaxcnnzup.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.vqdsnc.cn/gtwmxyompt.html

[T58] Scala：函数定义
来源：http://hz.cdnleiting.top/gteinelugx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ywan-chungtsiang.top/gtjodglhbp.html

[T59] Scala：循环
来源：http://hz.xylfe.cn/gtzzyharvk.html

for (i <- 1 to 10) println(i)
来源：http://hz.jinyuanbaomall.cn/gtenmgjunt.html

[T60] Scala：折叠
来源：http://hz.yuanzhike.top/gticjatjik.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cucudq.cn/gtvvurbhgx.html

================================================================================
来源：http://hz.mhx1999.top/gthixdlikl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.aizwys.cn/gtqhptwydw.html

================================================================================
来源：http://hz.fzhhl.top/gttxlpslyv.html

[U01] Py：创建虚拟环境
来源：http://hz.nwbrower.top/gtnsfxyftc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sxryk.cn/gthzdogabv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shanyushiyangtech.top/gthjhcprmq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gaohongyu789.top/gtfcvzvxqw.html

[U03] Py：加载 .env 配置
来源：http://hz.nanxuanxn.top/gtknijhacj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hammf.cn/gthhqixeyp.html

[U04] Py：变量调试打印
来源：http://hz.zhiwuduotai.top/gtjeostrby.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gotoacloud.top/gtgvkoodkr.html

[U05] Py：列表去重且保序
来源：http://hz.shanyushiyangkeji.top/gtplfanhpg.html

list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gttaccnrbg.html

[U06] Py：合并两个字典
来源：http://hz.52xcode.cn/gtzbmxoyqt.html

{**a, **b}
来源：http://hz.daria6918.cn/gtbbxbpmwu.html

[U07] Py：反转字典键值
来源：http://hz.chenjidiqi.icu/gtcpfvlbvn.html

{v: k for k, v in d.items()}
来源：http://hz.meibo888.top/gtlhpyxidq.html

[U08] Py：展平二维列表
来源：http://hz.hfpthk.cn/gtrdetfzbv.html

[y for x in nested for y in x]
来源：http://hz.9152youxi.cn/gthgwjaemb.html

[U09] Py：字典取最大值的键
来源：http://hz.andypj.xyz/gtnvyfiarm.html

max(d, key=d.get)
来源：http://hz.ehwqpu.com/gtxrqhawbu.html

[U10] Py：按值排序字典
来源：http://hz.yongpay.top/gtarvuiald.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sweek.top/gtistpvqex.html

[U11] Py：生成器表达式
来源：http://hz.nwbrower.top/gtvwxrcekc.html

(x * 2 for x in arr)
来源：http://hz.zhaomingkeji.xyz/gtxpapdxux.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.haohaochexian.top/gtivoqsfxw.html

Counter(arr).most_common(3)
来源：http://hz.xuanzx.com/gtgtgfqokw.html

[U13] Py：固定长度队列
来源：http://hz.snrcjt.cn/gtszfzemrn.html

deque(maxlen=10)
来源：http://hz.yonumen.top/gthlseqczq.html

[U14] Py：分组收集到列表
来源：http://hz.yueranfly.top/gtqosqdrks.html

defaultdict(list)
来源：http://hz.cheryme.top/gtmraicscz.html

[U15] Py：高精度计时
来源：http://hz.jianghu66.top/gtitvcbznj.html

t = time.perf_counter()
来源：http://hz.daxiang520.top/gtsckxgysn.html

[U16] Py：命令行参数解析
来源：http://hz.zhiwuduotai.top/gtacrgaekq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cucudq.cn/gtdchapray.html

[U17] Py：初始化日志
来源：http://hz.cucudq.cn/gthdaaplrg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.meibo888.top/gtvuvfqmkm.html

[U18] Py：预编译正则
来源：http://hz.jinghuilouyu.cn/gtvubrkpec.html

pat = re.compile(r"\d+")
来源：http://hz.aibaodan.cn/gtgqjdowmn.html

[U19] Py：正则替换带回调
来源：http://hz.pengpengdd.cyou/gttpnucomn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.andypj.xyz/gtiixnfurc.html

[U20] Py：缓存函数结果
来源：http://hz.ywan-chungtsiang.top/gtutrxaumm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hongshengwenyu.top/gterirfzli.html

[U21] Py：自定义上下文管理器
来源：http://hz.hnqzz.top/gtaojzdbhr.html

@contextlib.contextmanager
来源：http://hz.wangdashe.top/gtfnwcmxuy.html

[U22] Py：矩阵转置
来源：http://hz.xziqi.cn/gtsnuroiea.html

list(zip(*m))
来源：http://hz.nanxuanxn.top/gtqcjjsiln.html

[U23] Py：分块读取大文件
来源：http://hz.zdqjudy.top/gtgvsklgou.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yuanzhike.top/gtqvedtztg.html

[U24] Py：路径操作
来源：http://hz.quarkkingdee.top/gtrmmajlvr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.nwbrower.top/gtazqjmlml.html

[U25] Py：CSV 按字典读
来源：http://hz.zhaomingkeji.xyz/gtnlfdkcth.html

csv.DictReader(f)
来源：http://hz.jinghuilouyu.cn/gtrlfnsslr.html

[U26] Py：并发下载
来源：http://hz.chenjidiqi.icu/gtdgashhzr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zdqjudy.top/gtzezhimmd.html

[U27] Py：异步 HTTP
来源：http://hz.shanyushiyangkeji.top/gtegsrvpnm.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.wangdashe.top/gtnqpkuukw.html

[U28] Py：类型别名
来源：http://hz.chenzaomai.com/gtqpnqmxhk.html

UserId = int
来源：http://hz.zhijiandao.cn/gtpmbvhyao.html

[U29] Py：属性校验
来源：http://hz.mhx1999.top/gtbhvcfgwb.html

@property 与 @x.setter 配合
来源：http://hz.yj20258.top/gtjjqtqatg.html

[U30] Py：数据类
来源：http://hz.chenzaomai.com/gtxorsaidp.html

@dataclass(slots=True)
来源：http://hz.zhiwuduotai.top/gtbgbwvuzj.html

[U31] Py：单测
来源：http://hz.jinqigfzy.top/gtmqlksril.html

python -m pytest -q
来源：http://hz.zhaomingkeji.xyz/gttvbhfzuf.html

[U32] Py：代码格式化
来源：http://hz.9152youxi.cn/gtwvsmjtxr.html

ruff format . && ruff check --fix .
来源：http://hz.jlsjyb.cn/gtujtisgmv.html

[U33] Py：打包发布
来源：http://hz.hnqzz.top/gtelrzpbdw.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.chenlongwang.top/gtwcimeldi.html

[U34] Py：判断编码
来源：http://hz.aibaodan.cn/gtohkvemwt.html

chardet.detect(raw)
来源：http://hz.jqgufenzy.top/gtvyeesqdt.html

[U35] Py：发送邮件
来源：http://hz.nwbrower.top/gtckcclgmq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ydzc1.top/gtdjkcxrnj.html

[U36] Py：定时任务
来源：http://hz.jqgufenzy.top/gtvujprnqn.html

schedule.every(10).minutes.do(job)
来源：http://hz.cashguo.top/gtwlzfddlo.html

[U37] Py：读写 Excel
来源：http://hz.zhaomingkeji.xyz/gtqczszpog.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhongyouzk.top/gtgtdymhlr.html

[U38] Py：获取脚本所在目录
来源：http://hz.yangfankeji.com/gtqxqdonzl.html

Path(__file__).resolve().parent
来源：http://hz.sxryk.cn/gtclyfpjdi.html

[U39] Py：判断是否在交互环境
来源：http://hz.xingfuxueyuan.xyz/gtgcnzrumd.html

sys.stdout.isatty()
来源：http://hz.guannengcc.top/gtgieaxixm.html

[U40] Py：打印到标准错误
来源：http://hz.aizwys.cn/gtbsgifgkh.html

print("err", file=sys.stderr)
来源：http://hz.yj20258.top/gtjcygsjlt.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.daria6918.cn/gtgowaadrg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yongpay.top/gtnijtkcnb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhongyouzk.top/gtmmycisnm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ywan-chungtsiang.top/gtjdreysek.html

[U43] PHP：声明命名空间
来源：http://hz.ppjwa.cn/gtsetryinz.html

namespace App\Http;
来源：http://hz.cdnleiting.top/gtbihxemlk.html

[U44] PHP：开启严格类型
来源：http://hz.chenjidiqi.icu/gtmfwyfsad.html

declare(strict_types=1);
来源：http://hz.fengsongda.top/gtweopmdop.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yvedp.cn/gtrnnbptpz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.9152youxi.cn/gtrouyovvp.html

[U46] PHP：可空类型
来源：http://hz.kuanghao11.cn/gthpcxwdse.html

?string $name = null
来源：http://hz.feifeiyinyue.top/gtnagpqyot.html

[U47] PHP：联合类型
来源：http://hz.aizwys.cn/gtsdybknga.html

int|string $id
来源：http://hz.zhaomingkeji.xyz/gtsmoezuaw.html

[U48] PHP：纯枚举
来源：http://hz.gzhubu.top/gtoxuijdec.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gzhubu.top/gtrpbqtqld.html

[U49] PHP：只读属性
来源：http://hz.jinqigfzy.top/gtuwmvtwmn.html

public readonly string $name
来源：http://hz.feifeiyinyue.top/gtjlwaeeza.html

[U50] PHP：构造器属性提升
来源：http://hz.sufxvd.cn/gtdrfgqoae.html

public function __construct(private int $id) {}
来源：http://hz.ywan-chungtsiang.top/gtbqkvfdwh.html

[U51] PHP：数组解构
来源：http://hz.jqgufenzy.top/gtmbsyrgmo.html

[$a, $b] = $arr;
来源：http://hz.c1oappe.top/gttlytjykr.html

[U52] PHP：箭头函数
来源：http://hz.ivvv.top/gtjngifkmw.html

$double = fn($x) => $x * 2;
来源：http://hz.jqgufenzy.top/gtkdcjecog.html

[U53] PHP：空合并运算符
来源：http://hz.cqqwz.cn/gttvuogpkf.html

$v = $a ?? $b ?? "default";
来源：http://hz.xuetiantiany.cn/gtklhgwdwo.html

[U54] PHP：空安全调用
来源：http://hz.sxryk.cn/gtjobpprye.html

$obj?->method()
来源：http://hz.ybcxt.top/gtoezasbcu.html

[U55] PHP：match 表达式
来源：http://hz.sysykeji.top/gtzmsyifcw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jinyuanbaomall.cn/gtxkldsmzw.html

[U56] PHP：命名参数
来源：http://hz.haohaochexian.top/gtcfivwczo.html

f(a: 1, b: 2)
来源：http://hz.yuxming.cn/gtnaprnxor.html

[U57] PHP：字符串插值
来源：http://hz.cqqwz.cn/gtxgehbcbn.html

"值: {$a}"
来源：http://hz.mhx1999.top/gtxjjfrsjg.html

[U58] PHP：数组三件套
来源：http://hz.redwolf501.top/gtlitsemrb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.pengpengdd.cyou/gtqfaxugrx.html

[U59] PHP：自定义排序
来源：http://hz.zhiwuduotai.top/gtlnbvrcqc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhengqikj.top/gtngswerdi.html

[U60] PHP：JSON 编解码
来源：http://hz.wangdashe.top/gtpfpeuaqm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yuxming.cn/gtgnczxpbe.html

[U61] PHP：正则
来源：http://hz.wangdashe.top/gtntxyryuz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtfvzroaub.html

[U62] PHP：日期对象
来源：http://hz.316326.xyz/gtpcwydqvo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.havefunace.top/gteolrufpa.html

[U63] PHP：文件读写
来源：http://hz.yangfankeji.com/gtjoaukoih.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xylfe.cn/gtibzzjmup.html

[U64] PHP：目录遍历
来源：http://hz.tianlin.xyz/gtsqilnzkj.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xuetiantiany.cn/gthqsiatcn.html


<!-- 参考信息 -->